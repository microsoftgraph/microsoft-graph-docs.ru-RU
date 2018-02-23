# <a name="iosnotificationsettings-resource-type"></a><span data-ttu-id="98adc-101">Тип ресурса iosNotificationSettings</span><span class="sxs-lookup"><span data-stu-id="98adc-101">iosNotificationSettings resource type</span></span>

> <span data-ttu-id="98adc-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="98adc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98adc-103">Элемент, описывающий параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="98adc-103">An item describing notification setting.</span></span>
## <a name="properties"></a><span data-ttu-id="98adc-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="98adc-104">Properties</span></span>
|<span data-ttu-id="98adc-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="98adc-105">Property</span></span>|<span data-ttu-id="98adc-106">Тип</span><span class="sxs-lookup"><span data-stu-id="98adc-106">Type</span></span>|<span data-ttu-id="98adc-107">Описание</span><span class="sxs-lookup"><span data-stu-id="98adc-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98adc-108">bundleID</span><span class="sxs-lookup"><span data-stu-id="98adc-108">bundleID</span></span>|<span data-ttu-id="98adc-109">String</span><span class="sxs-lookup"><span data-stu-id="98adc-109">String</span></span>|<span data-ttu-id="98adc-110">Идентификатор пакета для приложения, к которому необходимо применить эти параметры уведомлений.</span><span class="sxs-lookup"><span data-stu-id="98adc-110">Bundle id of app to which to apply these notification settings.</span></span>|
|<span data-ttu-id="98adc-111">appName</span><span class="sxs-lookup"><span data-stu-id="98adc-111">appname</span></span>|<span data-ttu-id="98adc-112">String</span><span class="sxs-lookup"><span data-stu-id="98adc-112">String</span></span>|<span data-ttu-id="98adc-113">Имя приложения, которое нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="98adc-113">Application name to be associated with the bundleID.</span></span>|
|<span data-ttu-id="98adc-114">publisher</span><span class="sxs-lookup"><span data-stu-id="98adc-114">Publisher</span></span>|<span data-ttu-id="98adc-115">String</span><span class="sxs-lookup"><span data-stu-id="98adc-115">String</span></span>|<span data-ttu-id="98adc-116">Издатель, которого нужно связать со свойством bundleID.</span><span class="sxs-lookup"><span data-stu-id="98adc-116">Publisher to be associated with the bundleID.</span></span>|
|<span data-ttu-id="98adc-117">enabled</span><span class="sxs-lookup"><span data-stu-id="98adc-117">enabled</span></span>|<span data-ttu-id="98adc-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="98adc-118">Boolean</span></span>|<span data-ttu-id="98adc-119">Указывает, разрешены ли уведомления для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="98adc-119">Indicates whether notifications are allowed for this app.</span></span>|
|<span data-ttu-id="98adc-120">showInNotificationCenter</span><span class="sxs-lookup"><span data-stu-id="98adc-120">showInNotificationCenter</span></span>|<span data-ttu-id="98adc-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="98adc-121">Boolean</span></span>|<span data-ttu-id="98adc-122">Указывает, можно ли отображать уведомления в центре уведомлений.</span><span class="sxs-lookup"><span data-stu-id="98adc-122">Indicates whether notifications can be shown in notification center.</span></span>|
|<span data-ttu-id="98adc-123">showOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="98adc-123">showOnLockScreen</span></span>|<span data-ttu-id="98adc-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="98adc-124">Boolean</span></span>|<span data-ttu-id="98adc-125">Указывает, можно ли отображать уведомления на экране блокировки.</span><span class="sxs-lookup"><span data-stu-id="98adc-125">Indicates whether notifications can be shown on the lock screen.</span></span>|
|<span data-ttu-id="98adc-126">alertType</span><span class="sxs-lookup"><span data-stu-id="98adc-126">alertType</span></span>|<span data-ttu-id="98adc-127">String</span><span class="sxs-lookup"><span data-stu-id="98adc-127">String</span></span>|<span data-ttu-id="98adc-128">Определяет тип оповещения для уведомлений, связанных с этим приложением.</span><span class="sxs-lookup"><span data-stu-id="98adc-128">Indicates the type of alert for notifications for this app.</span></span> <span data-ttu-id="98adc-129">Возможные значения: `deviceDefault`, `banner`, `modal`, `none`.</span><span class="sxs-lookup"><span data-stu-id="98adc-129">Possible values are: `deviceDefault`, `banner`, `modal`, `none`.</span></span>|
|<span data-ttu-id="98adc-130">badgesEnabled</span><span class="sxs-lookup"><span data-stu-id="98adc-130">badgesEnabled</span></span>|<span data-ttu-id="98adc-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="98adc-131">Boolean</span></span>|<span data-ttu-id="98adc-132">Указывает, разрешены ли эмблемы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="98adc-132">Indicates whether badges are allowed for this app.</span></span>|
|<span data-ttu-id="98adc-133">soundsEnabled</span><span class="sxs-lookup"><span data-stu-id="98adc-133">soundsEnabled</span></span>|<span data-ttu-id="98adc-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="98adc-134">Boolean</span></span>|<span data-ttu-id="98adc-135">Указывает, разрешены ли звуковые сигналы для этого приложения.</span><span class="sxs-lookup"><span data-stu-id="98adc-135">Indicates whether sounds are allowed for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98adc-136">Связи</span><span class="sxs-lookup"><span data-stu-id="98adc-136">Relationships</span></span>
<span data-ttu-id="98adc-137">Нет</span><span class="sxs-lookup"><span data-stu-id="98adc-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98adc-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98adc-138">JSON Representation</span></span>
<span data-ttu-id="98adc-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98adc-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosNotificationSettings"
}
-->
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



