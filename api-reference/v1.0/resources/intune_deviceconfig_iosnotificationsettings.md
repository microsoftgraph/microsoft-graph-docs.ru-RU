# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="88316-101">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="88316-101">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="88316-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="88316-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88316-103">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="88316-103">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="88316-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="88316-104">Properties</span></span>
|<span data-ttu-id="88316-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="88316-105">Property</span></span>|<span data-ttu-id="88316-106">Тип</span><span class="sxs-lookup"><span data-stu-id="88316-106">Type</span></span>|<span data-ttu-id="88316-107">Описание</span><span class="sxs-lookup"><span data-stu-id="88316-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88316-108">bundleID</span><span class="sxs-lookup"><span data-stu-id="88316-108">bundleID</span></span>|<span data-ttu-id="88316-109">Строка</span><span class="sxs-lookup"><span data-stu-id="88316-109">String</span></span>|<span data-ttu-id="88316-110">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="88316-110">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="88316-111">appName</span><span class="sxs-lookup"><span data-stu-id="88316-111">appName</span></span>|<span data-ttu-id="88316-112">Строка</span><span class="sxs-lookup"><span data-stu-id="88316-112">String</span></span>|<span data-ttu-id="88316-113">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="88316-113">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="88316-114">publisher</span><span class="sxs-lookup"><span data-stu-id="88316-114">publisher</span></span>|<span data-ttu-id="88316-115">Строка</span><span class="sxs-lookup"><span data-stu-id="88316-115">String</span></span>|<span data-ttu-id="88316-116">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="88316-116">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="88316-117">enabled</span><span class="sxs-lookup"><span data-stu-id="88316-117">enabled</span></span>|<span data-ttu-id="88316-118">Логический</span><span class="sxs-lookup"><span data-stu-id="88316-118">Boolean</span></span>|<span data-ttu-id="88316-119">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="88316-119">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="88316-120">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="88316-120">showInNotificationCenter</span></span>|<span data-ttu-id="88316-121">Логический</span><span class="sxs-lookup"><span data-stu-id="88316-121">Boolean</span></span>|<span data-ttu-id="88316-122">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="88316-122">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="88316-123">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="88316-123">showOnLockScreen</span></span>|<span data-ttu-id="88316-124">Логический</span><span class="sxs-lookup"><span data-stu-id="88316-124">Boolean</span></span>|<span data-ttu-id="88316-125">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="88316-125">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="88316-126">alertType</span><span class="sxs-lookup"><span data-stu-id="88316-126">alertType</span></span>|[<span data-ttu-id="88316-127">iosNotificationAlertType</span><span class="sxs-lookup"><span data-stu-id="88316-127">iosNotificationAlertType values</span></span>](../resources/intune_deviceconfig_iosnotificationalerttype.md)|<span data-ttu-id="88316-128">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="88316-128">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="88316-129">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="88316-129">The possible values are `deviceDefault`, `banner`, `modal`, `none`, , , , , , , , or .</span></span>|
|<span data-ttu-id="88316-130">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="88316-130">badgesEnabled</span></span>|<span data-ttu-id="88316-131">Логический</span><span class="sxs-lookup"><span data-stu-id="88316-131">Boolean</span></span>|<span data-ttu-id="88316-132">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="88316-132">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="88316-133">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="88316-133">soundsEnabled</span></span>|<span data-ttu-id="88316-134">Логический</span><span class="sxs-lookup"><span data-stu-id="88316-134">Boolean</span></span>|<span data-ttu-id="88316-135">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="88316-135">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88316-136">Связи</span><span class="sxs-lookup"><span data-stu-id="88316-136">Relationships</span></span>
<span data-ttu-id="88316-137">Нет</span><span class="sxs-lookup"><span data-stu-id="88316-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="88316-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88316-138">JSON Representation</span></span>
<span data-ttu-id="88316-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88316-139">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNotificationSettings",
  "bundleID": "String",
  "appName": "String",
  "publisher": "String",
  "enabled": true,
  "showInNotificationCenter": true,
  "showOnLockScreen": true,
  "alertType": "String",
  "badgesEnabled": true,
  "soundsEnabled": true
}
```



