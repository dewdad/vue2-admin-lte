<template>
  <div>
    <div class="box box-default color-palette-box">
      <div class="box-header with-border">
        <h3 class="box-title"><i class="fa fa-tag"></i> Color Palette</h3>
      </div>
      <div class="box-body">
        <div class="row">
          <ColorPaletteSet v-for="color in colors[0]"
            :color="color"
          ></ColorPaletteSet>
        </div>
        <!-- /.row -->
        <div class="row">
          <ColorPaletteSet v-for="color in colors[1]"
            :color="color"
          ></ColorPaletteSet>
        </div>
        <!-- /.row -->
      </div>
    </div>

    <h2 class="page-header">Alerts and Callouts</h2>

    <div class="row">
      <div class="col-md-6">
        <div class="box box-default">
          <div class="box-header with-border">
            <i class="fa fa-warning"></i>

            <h3 class="box-title">Alerts</h3>
          </div>
          <!-- /.box-header -->
          <div class="box-body">

            <Alert
              type="danger"
              :dismissible="true">
              <div slot="header">
                <h4><i class="icon fa fa-ban"></i> Alert!</h4>
              </div>
              <div slot="body">
                Danger alert preview. This alert is dismissable. A wonderful serenity has taken possession of my entire
                soul, like these sweet mornings of spring which I enjoy with my whole heart.
              </div>
            </Alert>
            <Alert
              type="info"
              :dismissible="true">
              <div slot="header">
                <h4><i class="icon fa fa-info"></i> Alert!</h4>
              </div>
              <div slot="body">
                Info alert preview. This alert is dismissable.
              </div>
            </Alert>
            <Alert
              type="warning"
              :dismissible="true">
              <div slot="header">
                <h4><i class="icon fa fa-warning"></i> Alert!</h4>
              </div>
              <div slot="body">
                Warning alert preview. This alert is dismissable.
              </div>
            </Alert>
            <Alert
              type="success"
              :dismissible="true">
              <div slot="header">
                <h4><i class="icon fa fa-check"></i> Alert!</h4>
              </div>
              <div slot="body">
                Success alert preview. This alert is dismissable.
              </div>
            </Alert>

          </div>
          <!-- /.box-body -->
        </div>
        <!-- /.box -->

      </div>

      <div class="col-md-6">
        <div class="box box-default">
          <div class="box-header with-border">
            <i class="fa fa-bullhorn"></i>

            <h3 class="box-title">Callouts</h3>
          </div>
          <!-- /.box-header -->
          <div class="box-body">

            <Callout
              type="danger"
              title="I am a danger callout!"
              text="There is a problem that we need to fix. A wonderful serenity has taken possession of my entire soul, like these sweet mornings of spring which I enjoy with my whole heart."
            ></Callout>

            <Callout
              type="info"
              title="I am an info callout!"
              text="Follow the steps to continue to payment."
            ></Callout>

            <Callout
              type="warning"
              title="I am a warning callout!"
              text="This is a yellow callout."
            ></Callout>

            <Callout
              type="success"
              title="I am a success callout!"
              text="This is a green callout."
            ></Callout>

          </div>
          <!-- /.box-body -->
        </div>
        <!-- /.box -->
      </div>
      <!-- /.col -->
    </div>

    <h2 class="page-header">AdminLTE Custom Tabs</h2>

    <div class="row">
      <div class="col-md-6">

        <CustomTab>

          <li slot="nav"
              class="dropdown">
            <a class="dropdown-toggle"
              data-toggle="dropdown"
              href="#">
                                    Dropdown <span class="caret"></span>
                                  </a>
            <ul class="dropdown-menu">
              <li role="presentation"><a role="menuitem"
                  tabindex="-1"
                  href="#">Action</a></li>
              <li role="presentation"><a role="menuitem"
                  tabindex="-1"
                  href="#">Another action</a></li>
              <li role="presentation"><a role="menuitem"
                  tabindex="-1"
                  href="#">Something else here</a></li>
              <li role="presentation"
                  class="divider"></li>
              <li role="presentation"><a role="menuitem"
                  tabindex="-1"
                  href="#">Separated link</a></li>
            </ul>
          </li>

          <li slot="nav"
              class="pull-right"><a href="#"
              class="text-muted"><i class="fa fa-gear"></i></a></li>

          <div slot="content"
              class="active"
              id="tab_1"
              title="Tab 1">
            <b>How to use:</b>

            <p>Exactly like the original bootstrap tabs except you should use the custom wrapper <code>.nav-tabs-custom</code> to achieve this style.</p>
            A wonderful serenity has taken possession of my entire soul, like these sweet mornings of spring which I enjoy with my whole heart. I am alone, and feel the charm of existence in this spot, which was created for the bliss of souls like mine. I am so happy, my dear friend, so absorbed in the exquisite sense of mere tranquil existence, that I neglect my talents. I should be incapable of drawing a single stroke at the present moment; and yet I feel that I never was a greater artist than now.
          </div>
          <!-- /.tab-pane -->
          <div slot="content"
              id="tab_2"
              title="Tab 2">
            The European languages are members of the same family. Their separate existence is a myth. For science, music, sport, etc, Europe uses the same vocabulary. The languages only differ in their grammar, their pronunciation and their most common words. Everyone realizes why a new common language would be desirable: one could refuse to pay expensive translators. To achieve this, it would be necessary to have uniform grammar, pronunciation and more common words. If several languages coalesce, the grammar of the resulting language is more simple and regular than that of the individual languages.
          </div>
          <!-- /.tab-pane -->
          <div slot="content"
              id="tab_3"
              title="Tab 3">
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
          </div>
          <!-- /.tab-pane -->

        </CustomTab>

      </div>


      <div class="col-md-6">

        <CustomTab
          tabsClass="pull-right"
        >

          <li slot="nav"
              class="dropdown">
            <a class="dropdown-toggle"
              data-toggle="dropdown"
              href="#">
              Dropdown <span class="caret"></span>
            </a>
            <ul class="dropdown-menu">
              <li role="presentation"><a role="menuitem"
                  tabindex="-1"
                  href="#">Action</a></li>
              <li role="presentation"><a role="menuitem"
                  tabindex="-1"
                  href="#">Another action</a></li>
              <li role="presentation"><a role="menuitem"
                  tabindex="-1"
                  href="#">Something else here</a></li>
              <li role="presentation"
                  class="divider"></li>
              <li role="presentation"><a role="menuitem"
                  tabindex="-1"
                  href="#">Separated link</a></li>
            </ul>
          </li>

          <li slot="nav" class="pull-left header"><i class="fa fa-th"></i> Custom Tabs</li>


          <div slot="content"
              class="active"
              id="tab_1"
              title="Tab 1">
            <b>How to use:</b>

            <p>Exactly like the original bootstrap tabs except you should use the custom wrapper <code>.nav-tabs-custom</code> to achieve this style.</p>
            A wonderful serenity has taken possession of my entire soul, like these sweet mornings of spring which I enjoy with my whole heart. I am alone, and feel the charm of existence in this spot, which was created for the bliss of souls like mine. I am so happy, my dear friend, so absorbed in the exquisite sense of mere tranquil existence, that I neglect my talents. I should be incapable of drawing a single stroke at the present moment; and yet I feel that I never was a greater artist than now.
          </div>
          <!-- /.tab-pane -->
          <div slot="content"
              id="tab_2"
              title="Tab 2">
            The European languages are members of the same family. Their separate existence is a myth. For science, music, sport, etc, Europe uses the same vocabulary. The languages only differ in their grammar, their pronunciation and their most common words. Everyone realizes why a new common language would be desirable: one could refuse to pay expensive translators. To achieve this, it would be necessary to have uniform grammar, pronunciation and more common words. If several languages coalesce, the grammar of the resulting language is more simple and regular than that of the individual languages.
          </div>
          <!-- /.tab-pane -->
          <div slot="content"
              id="tab_3"
              title="Tab 3">
            Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
          </div>
          <!-- /.tab-pane -->

        </CustomTab>

      </div>

    </div>

    <h2>Progress Bars</h2>

    <div class="row">

      <div class="col-md-6">

        <Box
          title="Progress Bars Different Sizes"
          :isBorder="true"
          widgetType=""
        >
          <div slot="content">

            <p><code>.progress</code></p>
            <ProgressBar
              type="primary"
              :max="100"
              :value="40"
              text="40% Complete (success)"
            >
            </ProgressBar>

            <p>Class: <code>.sm</code></p>
            <ProgressBar
              type="success"
              size="sm"
              :max="100"
              :value="20"
              :isActive="true"
              text="20% Complete">
            </ProgressBar>

            <p>Class: <code>.xs</code></p>
            <ProgressBar
              type="warning"
              size="xs"
              :max="100"
              :value="60"
              text="60% Complete (warning)">
            </ProgressBar>

            <p>Class: <code>.xxs</code></p>
            <ProgressBar
              type="danger"
              size="xxs"
              :max="100"
              :value="60"
              text="60% Complete (danger)">
            </ProgressBar>

          </div>
        </Box>

      </div>


      <div class="col-md-6">


        <Box
          title="Progress bars"
          :isBorder="true"
          widgetType=""
          >
          <div slot="content">


            <ProgressBar
              type="green"
              :isStriped="false"
              :max="100"
              :value="40"
              text="40% Complete (success)">
            </ProgressBar>


            <ProgressBar
              type="aqua"
              :isStriped="false"
              :max="100"
              :value="20"
              text="20% Complete">
            </ProgressBar>


            <ProgressBar
              type="yellow"
              :isStriped="false"
              :max="100"
              :value="60"
              text="60% Complete (warning)">
            </ProgressBar>


            <ProgressBar
              type="red"
              :isStriped="false"
              :max="100"
              :value="80"
              text="80% Complete">
            </ProgressBar>


          </div>
        </Box>


      </div>

    </div>

    <div class="row">

      <div class="col-md-6">

        <Box title="Vertical Progress Bars Different Sizes"
            :isBorder="true"
            widgetType="">
          <div slot="content" class="text-center">

            <p>By adding the class <code>.vertical</code> and <code>.progress-sm</code>, <code>.progress-xs</code> or
              <code>.progress-xxs</code> we achieve:</p>


            <ProgressBar
              type="primary"
              :max="100"
              :value="40"
              :isActive="true"
              :isVertical="true"
              text="40%">
            </ProgressBar>


            <ProgressBar
              type="success"
              size="sm"
              :max="100"
              :value="20"
              :isActive="true"
              :isVertical="true"
              text="20%">
            </ProgressBar>


            <ProgressBar
              type="warning"
              size="xs"
              :max="100"
              :value="60"
              :isActive="true"
              :isVertical="true"
              text="60%">
            </ProgressBar>


            <ProgressBar
              type="info"
              size="xxs"
              :max="100"
              :value="60"
              :isActive="true"
              :isVertical="true"
              text="60%">
            </ProgressBar>

          </div>
        </Box>
      </div>

      <div class="col-md-6">

        <Box
          title="Vertical Progress bars"
          :isBorder="true"
          widgetType="">
          <div slot="content" class="text-center">

            <p>By adding the class <code>.vertical</code> we achieve:</p>

            <ProgressBar
              type="green"
              :max="100"
              :value="40"
              :isStriped="false"
              :isVertical="true"
              text="40%">
            </ProgressBar>

            <ProgressBar
              type="aqua"
              :max="100"
              :value="20"
              :isStriped="false"
              :isVertical="true"
              text="20%">
            </ProgressBar>

            <ProgressBar
              type="yellow"
              :max="100"
              :value="60"
              :isStriped="false"
              :isVertical="true"
              text="60%">
            </ProgressBar>

            <ProgressBar
              type="red"
              :max="100"
              :value="60"
              :isStriped="false"
              :isVertical="true"
              text="60%">
            </ProgressBar>

          </div>
        </Box>
      </div>


    </div>

  </div>

</template>

<script>
import ColorPaletteSet from '../../components/ColorPaletteSet.vue'
import Alert from '../../components/Alert.vue'
import Callout from '../../components/Callout.vue'
import CustomTab from '../../components/CustomTab.vue'
import Box from '../../widgets/Box.vue'
import ProgressBar from '../../components/ProgressBar.vue'

export default {
  name: 'General',
  data () {
    return {
      colors: [
        ['Primary', 'Info', 'Success', 'Warning', 'Danger', 'Gray'],
        ['Navi', 'Teal', 'Purple', 'Orange', 'Maroon', 'Black']
      ]
    }
  },
  created () {

  },
  components: {
    ColorPaletteSet,
    Alert,
    Callout,
    CustomTab,
    Box,
    ProgressBar
  }
}
</script>

<style>

.color-palette {
  height: 35px;
  line-height: 35px;
  text-align: center;
}

.color-palette-set {
  margin-bottom: 15px;
}

.color-palette span {
  display: none;
  font-size: 12px;
}

.color-palette:hover span {
  display: block;
}

.color-palette-box h4 {
  position: absolute;
  top: 100%;
  left: 25px;
  margin-top: -40px;
  color: rgba(255, 255, 255, 0.8);
  font-size: 12px;
  display: block;
  z-index: 7;
}

</style>
