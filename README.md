# Three.jsPractices

### Tutorials I used:
  - http://www.hewebgl.com/article/articledir/1
  - https://threejs.org/docs/index.html#manual/en/introduction/Creating-a-scene
  - https://www.udacity.com/course/interactive-3d-graphics--cs291
  - https://read.douban.com/reader/ebook/7412854/
  

### Three.js 功能概况
  
Cameras（照相机，控制投影方式）

    Camera
    OrthographicCamera （正交投影）
         THREE.OrthographicCamera(left, right, top, bottom, near, far)
        （横向缩小 可视放大 位置右移 可视左移）
         
    PerspectiveCamera （透视投影）
         THREE.PerspectiveCamera(fov, aspect, near, far)
         (张角缩小 可视放大）

Core（核心对象）

    BufferGeometry
    Clock（用来记录时间）
    EventDispatcher
    Face3
    Face4
    Geometry
      THREE.CubeGeometry(width, height, depth, widthSegments, heightSegments, depthSegments)  
      （width:x height:y 后三个参数分别是在三个方向上的分段数，widthSegments为3的话，代表x方向上水平分为三份，只是面被分）
      THREE.PlaneGeometry(width, height, widthSegments, heightSegments)
      THREE.SphereGeometry(radius, segmentsWidth, segmentsHeight, phiStart, phiLength, thetaStart, thetaLength)
      （segmentsWidth经度上的切片数；segmentsHeight纬度上的切片数；phiStart经度开始的弧度；phiLength经度跨过的弧度；thetaStart纬度）
      THREE.CircleGeometry(radius, segments, thetaStart, thetaLength)
      THREE.CylinderGeometry(radiusTop, radiusBottom, height, radiusSegments, heightSegments, openEnded)
      THREE.TetrahedronGeometry(radius, detail)
      （正四面体）
      THREE.OctahedronGeometry(radius, detail)
      （正八面体）
      THREE.IcosahedronGeometry(radius, detail)
      THREE.TorusGeometry(radius, tube, radialSegments, tubularSegments, arc)
      （tube 管道半径 radialSegments管道小圆分 tubularSegments 大圆环分）
      THREE.TorusKnotGeometry(radius, tube, radialSegments, tubularSegments, p, q, heightScale)
    Object3D
    Projector
    Raycaster（计算鼠标拾取物体时很有用的对象）

Materials（材质，控制物体的颜色、纹理等）

    Material
    LineBasicMaterial
    LineDashedMaterial
    MeshBasicMaterial (始终为该材质的颜色，不会由于光照产生明暗、阴影效果)
    MeshDepthMaterial
    MeshFaceMaterial
    MeshLambertMaterial （考虑漫反射而不考虑镜面反射的效果，因而对于金属、镜子等需要镜面反射效果的物体就不适应）
    MeshNormalMaterial （将材质的颜色设置为其法向量的方向，对于调试很有帮助）
    MeshPhongMaterial (考虑漫反射高光 specular高光颜色 shininess越大光斑越小)
    ParticleBasicMaterial
    ParticleCanvasMaterial
    ParticleDOMMaterial
    ShaderMaterial
    SpriteMaterial

Lights（光照）

    Light
    AmbientLight
    AreaLight
    DirectionalLight
    HemisphereLight
    PointLight
    SpotLight

Loaders（加载器，用来加载特定文件）

    Loader
    BinaryLoader
    GeometryLoader
    ImageLoader
    JSONLoader
    LoadingMonitor
    SceneLoader
    TextureLoader

Math（和数学相关的对象）

    Box2
    Box3
    Color
    Frustum
    Math
    Matrix3
    Matrix4
    Plane
    Quaternion
    Ray
    Sphere
    Spline
    Triangle
    Vector2
    Vector3
    Vector4

Objects（物体）

    Bone
    Line
    LOD
    Mesh（网格，最常用的物体）
    MorphAnimMesh
    Particle
    ParticleSystem
    Ribbon
    SkinnedMesh
    Sprite

Renderers（渲染器，可以渲染到不同对象上）

    CanvasRenderer
    WebGLRenderer（使用WebGL渲染，这是本书中最常用的方式）
    WebGLRenderTarget
    WebGLRenderTargetCube
    WebGLShaders（着色器，在最后一章作介绍）

Renderers / Renderables

    RenderableFace3
    RenderableFace4
    RenderableLine
    RenderableObject
    RenderableParticle
    RenderableVertex

Scenes（场景）

    Fog
    FogExp2
    Scene

Textures（纹理）

    CompressedTexture
    DataTexture
    Texture

Extras

    FontUtils
    GeometryUtils
    ImageUtils
    SceneUtils

Extras / Animation

    Animation
    AnimationHandler
    AnimationMorphTarget
    KeyFrameAnimation

Extras / Cameras

    CombinedCamera
    CubeCamera

Extras / Core

    Curve
    CurvePath
    Gyroscope
    Path
    Shape

Extras / Geometries（几何形状）

    CircleGeometry
    ConvexGeometry
    CubeGeometry
    CylinderGeometry
    ExtrudeGeometry
    IcosahedronGeometry
    LatheGeometry
    OctahedronGeometry
    ParametricGeometry
    PlaneGeometry
    PolyhedronGeometry
    ShapeGeometry
    SphereGeometry
    TetrahedronGeometry
    TextGeometry
    TorusGeometry
    TorusKnotGeometry
    TubeGeometry

Extras / Helpers

    ArrowHelper
    AxisHelper
    CameraHelper
    DirectionalLightHelper
    HemisphereLightHelper
    PointLightHelper
    SpotLightHelper

Extras / Objects

    ImmediateRenderObject
    LensFlare
    MorphBlendMesh

Extras / Renderers / Plugins

    DepthPassPlugin
    LensFlarePlugin
    ShadowMapPlugin
    SpritePlugin

Extras / Shaders

    ShaderFlares
    ShaderSprite
