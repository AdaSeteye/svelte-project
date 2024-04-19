<!-- app.svelte -->
<script>
  import LeftPanel from "./LeftPanel.svelte";
  import RightPanel from "./RightPanel.svelte";
  import BottomPanel from "./BottomPanel.svelte";
</script>

<img src="/images/bird-image.jpg" alt="Bird" class="desktop-image" />

<div class="page-container">
  <div class="desktop-layout">
    <div class="left-panel">
      <LeftPanel />
    </div>
    <div class="separator"></div>
    <div class="right-panel">
      <RightPanel />
    </div>
  </div>
  <BottomPanel />
</div>

<style>
  .desktop-image {
    position: absolute;
    top: 10px;
    right: 10px;
    width: 20px;
    height: auto;
    background-color: rgb(7, 169, 223);
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
  }

  .page-container {
    max-width: 1200px;
    margin: 0 auto;
  }

  @media (min-width: 769px) {
    .page-container {
      margin: 40px 100px;
    }
  }

  .desktop-layout {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    padding: 20px;
  }

  .left-panel,
  .right-panel {
    width: 48%;
    height: 100%;
    box-sizing: border-box;
  }

  .separator {
    width: 4%;
  }

  @media (max-width: 768px) {
    .desktop-layout {
      flex-direction: column;
      align-items: center;
    }
    .left-panel,
    .right-panel {
      width: 100%;
      height: auto;
    }
    .separator {
      display: none;
    }
    .right-panel {
      order: -1;
    }
    .desktop-image {
      top: 0;
      right: calc(50% - 25px);
    }
  }

  @media (min-width: 769px) {
    .desktop-layout {
      flex-direction: row;
    }
    .left-panel,
    .right-panel {
      width: 48%;
    }
    .separator {
      width: 4%;
    }
  }
</style>
