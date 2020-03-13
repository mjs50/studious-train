/* Makes bookmarks toolbar span multiple rows, removes icon text, and puts rounded tabs at the bottom */

.tabbrowser-tab {
    box-sizing: border-box;
    margin: 0 1px 0 1px !important;
    border-radius: 5px 5px 0 0 !important;
}


.tabbrowser-tab .tab-text.tab-label {
    color: black !important;            /* tab text color - customizable */
}


.tabbrowser-tab[selected="true"] .tab-text.tab-label {
    color: black !important;            /* tab text color - customizable */
}


.tabbrowser-tab[selected="true"] .tab-background {
    border: 1px solid gray !important;  /* color is customizable */
    border-bottom: none !important;
    opacity: 1;
}

 
#tabbrowser-tabs {
  min-height: unset !important;
  padding-inline-start: 0px !important;
}



.tab-background {
    border: none !important;
    border-radius: 5px 5px 0 0 !important;
    background: black;
    opacity: .1;
}


.tab-line {                             /* = light top line in selected tab in Quantum default */
    display: none !important;
}


.tabbrowser-tab:hover,
.tabbrowser-tab .tab-text.tab-label:hover {
    cursor: pointer !important; 
}


.tabbrowser-tab:hover {
    border: 1px solid grey !important;
}


.tabbrowser-tab[selected="true"]:hover {
    border: none !important;
}


[tabsintitlebar]:root:not([extradragspace]) .tabbrowser-tab::after,
.tabbrowser-tab:hover::after,
#tabbrowser-tabs:not([movingtab])>.tabbrowser-tab[beforehovered]::after {
    border: none !important;                /* leave as is; affects the New Tab icon (the plus) */
}


/* BOOKMARK ICON COLORIZATION */

#bookmarks-view treechildren::-moz-tree-image(container),
#PlacesToolbarItems toolbarbutton[container="true"] .toolbarbutton-icon,
#PlacesToolbarItems menu[container="true"] .menu-iconic-left,
#BMB_bookmarksPopup menu[container="true"] .menu-iconic-icon,
#bookmarksMenu menu[container="true"] .menu-iconic-icon {
    fill: #FFCC00 !important;               /* orange; customizable */
    margin-right: 8px;                      /* correction for the Firefox default imperfection */
}


/* ADDRESS BAR ICONS CLEAN-UP */

#pageActionSeparator, #pocket-button, #pageActionButton {
    display: none !important;               /* customizable: delete if you want the objects back */
}

/* TABS on bottom */
#navigator-toolbox toolbar:not(#nav-bar):not(#toolbar-menubar) {
 -moz-box-ordinal-group: 10;
}
#TabsToolbar {
 -moz-box-ordinal-group: 1000 !important;
}

#TabsToolbar {
 display: block !important;
 position: absolute !important;
 bottom: 0 !important;
 width: 100vw !important;
}

#main-window:not([chromehidden*="toolbar"]) #navigator-toolbox {
 padding-bottom: var(--tab-min-height) !important;
}

#tabbrowser-tabs {
 width: 100vw !important;
}

#TabsToolbar #window-controls {
 display: none !important;
}



   at least a quarter second (250 milliseconds).
   Once shown on hover, they remain for 2 seconds
   after hover ends before collapsing out again.
*/
toolbarbutton.bookmark-item .toolbarbutton-text {
  visibility: collapse !important;
  opacity: 0 !important;
  transition: all 250ms 2s ease-in-out !important;
}
toolbarbutton.bookmark-item:hover .toolbarbutton-text {
  visibility: visible !important;
  opacity: 1 !important;
  transition: all 250ms 250ms ease-in-out !important;
}

/* Makes bookmarks toolbar span multiple rows */

#PersonalToolbar{
  --multirow-bmb-n-rows: 3; /* Control how many rows are shown before scrolling */
  --multirow-bmb-row-margin: 2px; /* Control how much spacing is between rows */
  max-height: none !important;
}

#PlacesToolbar > hbox{ 
  display: block;
  width: 100vw;
}

#PlacesToolbarItems{
  display: flex;
  flex-wrap: wrap;
  /* --uc-bm-padding is defined in autohide_bookmarks_toolbar.css */
  max-height: calc(var(--multirow-bmb-n-rows) * (5px + 1em + (2 * (var(--multirow-bmb-row-margin) + var(--uc-bm-padding,2px))))) !important;
  overflow-y:auto;
  scrollbar-color: var(--lwt-accent-color) var(--toolbar-bgcolor) ;
  scrollbar-width: thin;
}

/* Hide the all-bookmarks button */
#PlacesChevron{ display: none }

/* Add some spacing between rows */
#PlacesToolbarItems > .bookmark-item{ margin: var(--multirow-bmb-row-margin) 2px !important;  }

#personal-bookmarks .bookmark-item > .toolbarbutton-text { display:none !important; }
