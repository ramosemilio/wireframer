#WIREFRAMER v0.1
#By Emilio Ramos

import pymel.core as pm
import pymel.core.datatypes as dt
import pymel.core.windows as win

#-------------------------------------------------------------------------------
#-------------------------------------------------------------------------------
#GUI CODE
#-------------------------------------------------------------------------------
#-------------------------------------------------------------------------------

#CREATE NEW WINDOW
gui = pm.window(
    title="Wireframer v0.1",
    height=560,
    width=340,
    toolbox=True,
    sizeable=False,)

#CREATE GUI LAYOUT
template = win.uiTemplate("v0.1_Template")
template.define(
    win.frameLayout,
    borderVisible=True,
    width=300,
    marginHeight=10,
    marginWidth=10)

with template:
    #MAIN LAYOUT COLUMN
    with win.frameLayout(labelVisible=False, borderVisible=False):

        #NODE OPTIONS
        with win.frameLayout(label="Node Options"):
            with win.columnLayout(rowSpacing=10):
                #NODE GEOMETRY FIELD
                win.text(label="Node geometry:")
                with win.optionMenu(width=100) as node_geo_opt:
                    win.menuItem(label='Sphere')
                    win.menuItem(label='Tetrahedron')
                    win.menuItem(label='Cube')
                    win.menuItem(label='Octahedron')
                    win.menuItem(label='Dodecahedron')
                    win.menuItem(label='Icosohedron')
                #NODE SCALE FIELD
                win.text(label="Node scale:")
                with win.rowLayout(numberOfColumns=2):
                    node_scale_opt = win.floatField(
                        width=100,
                        editable=True,
                        maxValue=20.0,
                        minValue=0.1,
                        precision=2,
                        step=0.01,
                        value = 1.0,
                        changeCommand= lambda *args: n_slide_1.setValue(node_scale_opt.getValue())
                        )
                    n_slide_1 = win.floatSlider(
                        width=190,
                        maxValue=20.0,
                        minValue=0.1,
                        step=0.01,
                        value=1.0,
                        dragCommand= lambda *args: node_scale_opt.setValue(n_slide_1.getValue())
                        )
                #NODE SUBDIV FIELD
                win.text(label="Node subdivions:")
                with win.rowLayout(numberOfColumns=2):
                    node_subdiv_opt = win.intField(
                        width=100,
                        editable=True,
                        maxValue=16,
                        minValue=0,
                        step=1,
                        value = 1,
                        changeCommand= lambda *args: n_slide_2.setValue(node_subdiv_opt.getValue())
                        )
                    n_slide_2 = win.intSlider(
                        width=190,
                        maxValue=16,
                        minValue=0,
                        step=1,
                        value=1,
                        dragCommand= lambda *args: node_subdiv_opt.setValue(n_slide_2.getValue())
                        )

        #SPOKE OPTIONS
        with win.frameLayout("Spoke Options"):
            with win.columnLayout(rowSpacing=10):
                #SPOKE SIDES FIELD
                win.text(label="Spoke sides:")
                with win.rowLayout(numberOfColumns=2):
                    spoke_sides_opt = win.intField(
                        width=100,
                        editable=True,
                        maxValue=16,
                        minValue=3,
                        step=1,
                        value = 3,
                        changeCommand= lambda *args: s_slide_1.setValue(spoke_sides_opt.getValue())
                        )
                    s_slide_1 = win.intSlider(
                        width=190,
                        maxValue=16,
                        minValue=3,
                        step=1,
                        value=3,
                        dragCommand= lambda *args: spoke_sides_opt.setValue(s_slide_1.getValue())
                        )
                #SPOKE RADIUS FIELD
                win.text(label="Spoke radius:")
                with win.rowLayout(numberOfColumns=2):
                    spoke_radius_opt = win.floatField(
                        width=100,
                        editable=True,
                        maxValue=20.0,
                        minValue=0.1,
                        precision=2,
                        step=0.01,
                        value = 1.0,
                        changeCommand= lambda *args: s_slide_2.setValue(spoke_radius_opt.getValue())
                        )
                    s_slide_2 = win.floatSlider(
                        width=190,
                        maxValue=20.0,
                        minValue=0.1,
                        step=0.01,
                        value=1.0,
                        dragCommand= lambda *args: spoke_radius_opt.setValue(s_slide_2.getValue())
                        )
                #SPOKE LENGTH SUBDIV FIELD
                win.text(label="Spoke length divisions:")
                with win.rowLayout(numberOfColumns=2):
                    spoke_length_div_opt = win.intField(
                        width=100,
                        editable=True,
                        maxValue=16,
                        minValue=0,
                        step=1,
                        value = 1,
                        changeCommand= lambda *args: s_slide_3.setValue(spoke_length_div_opt.getValue())
                        )
                    s_slide_3 = win.intSlider(
                        width=190,
                        maxValue=16,
                        minValue=0,
                        step=1,
                        value=1,
                        dragCommand= lambda *args: spoke_length_div_opt.setValue(s_slide_3.getValue())
                        )
                #SPOKE CAPS FIELD
                win.text(label="Spoke cap subdivisions:")
                with win.rowLayout(numberOfColumns=2):
                    spoke_subdiv_opt = win.intField(
                        width=100,
                        editable=True,
                        maxValue=4,
                        minValue=0,
                        step=1,
                        value = 1,
                        changeCommand= lambda *args: s_slide_4.setValue(spoke_subdiv_opt.getValue())
                        )
                    s_slide_4 = win.intSlider(
                        width=190,
                        maxValue=4,
                        minValue=0,
                        step=1,
                        value=1,
                        dragCommand= lambda *args: spoke_subdiv_opt.setValue(s_slide_4.getValue())
                        )

        #EXTRA OPTIONS
        with win.frameLayout("Extra Options"):
            with win.columnLayout(rowSpacing=10):
                win.text(label="Hide source mesh:")
                with win.optionMenu() as hide_opt:
                    win.menuItem(label='Yes')
                    win.menuItem(label='No')
                win.text(label="Create selection sets:")
                with win.optionMenu() as sel_sets_opt:
                    win.menuItem(label='None')
                    win.menuItem(label='Nodes')
                    win.menuItem(label='Spokes')
                    win.menuItem(label='Nodes and Spokes')
                win.text(label="Boolean Union output mesh: (Experimental/Unstable)")
                with win.optionMenu() as bool_opt:
                    win.menuItem(label='None')
                    win.menuItem(label='Boolean Union')

        #SUBMISSION BUTTON
        generate_button = win.button(
            label="Generate Wireframe",
            width=300,
            height=60)

#BUTTON SUBMISSION FUNCTION
def buttonPressed(*args):
    #GET USER INPUT FROM FIELDS AND PASS TO GENERATOR FUNCTION
    generate_wireframe(
        node_geo_opt.getValue(),
        node_scale_opt.getValue(),
        node_subdiv_opt.getValue(),
        spoke_sides_opt.getValue(),
        spoke_radius_opt.getValue(),
        spoke_length_div_opt.getValue(),
        spoke_subdiv_opt.getValue(),
        hide_opt.getValue(),
        bool_opt.getValue(),
        sel_sets_opt.getValue()
        )

#ADD SUBMISSION FUNCTION TO BUTTON
generate_button.setCommand(buttonPressed)
#DISPLAY GUI
gui.show()

#-------------------------------------------------------------------------------
#-------------------------------------------------------------------------------
#WIREFRAME GENERATION CODE
#-------------------------------------------------------------------------------
#-------------------------------------------------------------------------------
def generate_wireframe(
    node_geo,
    node_scale,
    node_subdiv,
    spoke_sides,
    spoke_radius,
    spoke_length_div,
    spoke_subdiv,
    hidden,
    merge_bool_op,
    sel_sets):
    #PRINT INPUT TO CONSOLE AND GENERATE GEOMETRY
    print "Generating wireframe with the following parameters:"
    print "Node geometry: "+str(node_geo)
    print "Node scale: "+str(node_scale)
    print "Node subdiv: "+str(node_subdiv)
    print "Spoke sides: "+str(spoke_sides)
    print "Spoke radius: "+str(spoke_radius)
    print "Spoke length div: "+str(spoke_length_div)
    print "Spoke subdiv: "+str(spoke_subdiv)
    print "Hide original: "+str(hidden)
    print "Bool option: "+str(merge_bool_op)
    print "Selection set option: "+str(sel_sets)

    #CREATE SELECTION SETS------------------------------------------------------
    ns_name = ""
    ss_name = ""
    bs_name = ""
    #CREATE SETS FROM USER OPTIONS
    if sel_sets == "Nodes":
        node_set = pm.sets(empty=True, name = "NODES_SET")
        ns_name = node_set.name()
    if sel_sets == "Spokes":
        spoke_set = pm.sets(empty=True, name = "SPOKES_SET")
        ss_name = spoke_set.name()
    #BOOLEAN OPERATION SYNTAX REQUIRES 2 MESHES (NODE AND SPOKES)
    #MAKE BOTH SETS IN THIS CASE AS WELL
    if sel_sets == "Nodes and Spokes" or "Boolean Union":
        node_set = pm.sets(empty=True, name = "NODES_SET")
        spoke_set = pm.sets(empty=True, name = "SPOKES_SET")
        ns_name = node_set.name()
        ss_name = spoke_set.name()

    #GET SELECTED MESH
    transform_node = pm.ls(selection=True)
    #FREEZE SCALE
    pm.makeIdentity(apply=True, scale=True)
    #GET SHAPE NODE
    shape_node = transform_node[0].getShape()

    #GET AND ENUMERATE MESH EDGES AND VERTS
    mesh_edges = [i for i in shape_node.e]
    num_edges = int(pm.polyEvaluate(edge=True))
    mesh_verts = [i for i in shape_node.vtx]
    num_verts = int(pm.polyEvaluate(vertex=True))

    #SPOKE GENERATION SECTION---------------------------------------------------
    for edge in mesh_edges:
        edge_length = edge.getLength()
        vtx_1_pos = edge.connectedVertices()[0].getPosition()
        vtx_2_pos = edge.connectedVertices()[1].getPosition()
        #GET SPOKE ORIENTATION
        spoke_axis = dt.Vector(
            (vtx_1_pos[0]-vtx_2_pos[0]),
            (vtx_1_pos[1]-vtx_2_pos[1]),
            (vtx_1_pos[2]-vtx_2_pos[2]))
        spoke_name = "spoke_"+str(num_edges)
        #MAKE SPOKE FROM USER OPTIONS
        new_spoke = pm.polyCylinder(
            axis = spoke_axis,
            constructionHistory = False,
            height = edge_length,
            radius = spoke_radius,
            subdivisionsAxis = spoke_sides,
            subdivisionsHeight = spoke_length_div,
            subdivisionsCaps = spoke_subdiv,
            name= spoke_name)
        #CLEAR SELECTION BEFORE MOVING SPOKE
        pm.select( clear=True )
        pm.select( spoke_name)
        #MOVE SPOKE
        new_pos = (
            (vtx_1_pos[0]+vtx_2_pos[0])/2,
            (vtx_1_pos[1]+vtx_2_pos[1])/2,
            (vtx_1_pos[2]+vtx_2_pos[2])/2,)
        pm.move(new_pos)

        #ADD SPOKE TRANSFORM NODE TO SETS IF THEY EXIST
        if pm.objExists(ss_name):
            pm.sets(spoke_set, addElement=new_spoke[0])
        if pm.objExists(bs_name):
            pm.sets(bool_set, addElement=new_spoke[0])
        num_edges= num_edges-1

    #NODE GENERATION SECTION----------------------------------------------------
    for vtx in mesh_verts:
        #GET NODE POS AND ORIENTATION
        vtx_pos = vtx.getPosition()
        node_axis = vtx.getNormal()
        node_name = "node_"+str(num_verts)
        #MAKE NODE FROM USER OPTIONS
        if node_geo == "Sphere":
            new_node = pm.polySphere(
                axis = node_axis,
                constructionHistory = False,
                radius = node_scale,
                subdivisionsAxis = node_subdiv,
                subdivisionsHeight = node_subdiv,
                subdivisionsX = node_subdiv,
                subdivisionsY = node_subdiv,
                name= node_name)
        if node_geo == "Tetrahedron":
            new_node = pm.polyPyramid(
                axis = node_axis,
                constructionHistory = False,
                numberOfSides = 3,
                sideLength = node_scale,
                subdivisionsCaps = node_subdiv,
                subdivisionsHeight = node_subdiv,
                name= node_name)
        if node_geo == "Cube":
            new_node = pm.polyCube(
                axis = node_axis,
                constructionHistory = False,
                depth = node_scale,
                height = node_scale,
                width = node_scale,
                subdivisionsDepth = node_subdiv,
                subdivisionsHeight = node_subdiv,
                subdivisionsWidth = node_subdiv,
                name= node_name)
        if node_geo == "Octahedron":
            new_node = pm.polyPlatonicSolid(
                axis = node_axis,
                constructionHistory = False,
                radius = node_scale,
                sideLength = node_scale,
                solidType = 2,
                #subdivisions = node_subdiv,
                name= node_name)
        if node_geo == "Dodecahedron":
            new_node = pm.polyPlatonicSolid(
                axis = node_axis,
                constructionHistory = False,
                radius = node_scale,
                sideLength = node_scale,
                solidType = 0,
                #subdivisions = node_subdiv,
                name= node_name)
        if node_geo == "Icosohedron":
            new_node = pm.polyPlatonicSolid(
                axis = node_axis,
                constructionHistory = False,
                radius = node_scale,
                sideLength = node_scale,
                solidType = 1,
                #subdivisions = node_subdiv,
                name= node_name)
        #CLEAR SELECTION BEFORE MOVING NODE
        pm.select(clear=True)
        pm.select(node_name)
        pm.move(vtx_pos)

        #ADD NODE TRANSFORM NODE TO SETS IF THEY EXIST
        if pm.objExists(ns_name):
            pm.sets(node_set, addElement=new_node[0])
        if pm.objExists(bs_name):
            pm.sets(bool_set, addElement=new_node[0])
        num_verts= num_verts-1

    #BOOLEAN UNION SECTION------------------------------------------------------
    if merge_bool_op == "Boolean Union":
        #SELECT ALL NODES AND MERGE TO ONE MESH
        pm.select(clear=True)
        pm.select(node_set)
        node_merge = pm.polyUnite(constructionHistory=False, name="Merged_Nodes")
        #SELECT ALL SPOKES AND MERGE TO ONE MESH
        pm.select(clear=True)
        pm.select(spoke_set)
        spoke_merge = pm.polyUnite(constructionHistory=False, name="Merged_Spokes")
        #BOOLEAN OPERATION
        poly_bool = pm.polyBoolOp(
            node_merge[0].name(),
            spoke_merge[0].name(),
            operation = 1,
            constructionHistory = False,
            name = "Merged_Wireframe"
        )

    #HIDE SOURCE GEOMETRY---------------------------------------------------
    if hidden:
        pm.hide(transform_node)

