# <a name="applepushnotificationcertificate-resource-type"></a><span data-ttu-id="6216b-101">Тип ресурса applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="6216b-101">applePushNotificationCertificate resource type</span></span>

> <span data-ttu-id="6216b-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6216b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6216b-103">Сертификат push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="6216b-103">Apple push notification certificate.</span></span>
## <a name="methods"></a><span data-ttu-id="6216b-104">Методы</span><span class="sxs-lookup"><span data-stu-id="6216b-104">Methods</span></span>
|<span data-ttu-id="6216b-105">Метод</span><span class="sxs-lookup"><span data-stu-id="6216b-105">Method</span></span>|<span data-ttu-id="6216b-106">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6216b-106">Return Type</span></span>|<span data-ttu-id="6216b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="6216b-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6216b-108">Получение объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="6216b-108">Get applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_get.md)|[<span data-ttu-id="6216b-109">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="6216b-109">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="6216b-110">Чтение свойств и связей объекта [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="6216b-110">Read properties and relationships of [plannerPlanDetails](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="6216b-111">Обновление объекта applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="6216b-111">Update applePushNotificationCertificate</span></span>](../api/intune_devices_applepushnotificationcertificate_update.md)|[<span data-ttu-id="6216b-112">applePushNotificationCertificate</span><span class="sxs-lookup"><span data-stu-id="6216b-112">applePushNotificationCertificate</span></span>](../resources/intune_devices_applepushnotificationcertificate.md)|<span data-ttu-id="6216b-113">Обновление свойств объекта [applePushNotificationCertificate](../resources/intune_devices_applepushnotificationcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="6216b-113">Update the properties of a [calendar](../resources/intune_devices_applepushnotificationcertificate.md) object.</span></span>|
|[<span data-ttu-id="6216b-114">Функция downloadApplePushNotificationCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="6216b-114">downloadApplePushNotificationCertificateSigningRequest function</span></span>](../api/intune_devices_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md)|<span data-ttu-id="6216b-115">String</span><span class="sxs-lookup"><span data-stu-id="6216b-115">String</span></span>|<span data-ttu-id="6216b-116">Скачивание запроса на подпись сертификата для push-уведомлений Apple</span><span class="sxs-lookup"><span data-stu-id="6216b-116">Download Apple push notification certificate signing request</span></span>|

## <a name="properties"></a><span data-ttu-id="6216b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="6216b-117">Properties</span></span>
|<span data-ttu-id="6216b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="6216b-118">Property</span></span>|<span data-ttu-id="6216b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="6216b-119">Type</span></span>|<span data-ttu-id="6216b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6216b-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6216b-121">id</span><span class="sxs-lookup"><span data-stu-id="6216b-121">id</span></span>|<span data-ttu-id="6216b-122">String</span><span class="sxs-lookup"><span data-stu-id="6216b-122">String</span></span>|<span data-ttu-id="6216b-123">Уникальный идентификатор сертификата</span><span class="sxs-lookup"><span data-stu-id="6216b-123">Unique Identifier for the certificate</span></span>|
|<span data-ttu-id="6216b-124">appleIdentifier</span><span class="sxs-lookup"><span data-stu-id="6216b-124">appleIdentifier</span></span>|<span data-ttu-id="6216b-125">String</span><span class="sxs-lookup"><span data-stu-id="6216b-125">String</span></span>|<span data-ttu-id="6216b-126">Идентификатор Apple Id учетной записи, используемой для создания push-сертификата MDM.</span><span class="sxs-lookup"><span data-stu-id="6216b-126">Apple Id of the account used to create the MDM push certificate.</span></span>|
|<span data-ttu-id="6216b-127">topicIdentifier</span><span class="sxs-lookup"><span data-stu-id="6216b-127">topicIdentifier</span></span>|<span data-ttu-id="6216b-128">String</span><span class="sxs-lookup"><span data-stu-id="6216b-128">String</span></span>|<span data-ttu-id="6216b-129">ИД темы.</span><span class="sxs-lookup"><span data-stu-id="6216b-129">Topic Id.</span></span>|
|<span data-ttu-id="6216b-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6216b-130">lastModifiedDateTime</span></span>|<span data-ttu-id="6216b-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6216b-131">DateTimeOffset</span></span>|<span data-ttu-id="6216b-132">Дата и время последнего изменения сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="6216b-132">Last modified date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="6216b-133">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6216b-133">expirationDateTime</span></span>|<span data-ttu-id="6216b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6216b-134">DateTimeOffset</span></span>|<span data-ttu-id="6216b-135">Дата и время окончания срока действия для сертификата push-уведомлений Apple.</span><span class="sxs-lookup"><span data-stu-id="6216b-135">The expiration date and time for Apple push notification certificate.</span></span>|
|<span data-ttu-id="6216b-136">certificate</span><span class="sxs-lookup"><span data-stu-id="6216b-136">ACS, certificate</span></span>|<span data-ttu-id="6216b-137">String</span><span class="sxs-lookup"><span data-stu-id="6216b-137">String</span></span>|<span data-ttu-id="6216b-138">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6216b-138">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="6216b-139">Связи</span><span class="sxs-lookup"><span data-stu-id="6216b-139">Relationships</span></span>
<span data-ttu-id="6216b-140">Нет</span><span class="sxs-lookup"><span data-stu-id="6216b-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6216b-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6216b-141">JSON Representation</span></span>
<span data-ttu-id="6216b-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6216b-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applePushNotificationCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
  "id": "String (identifier)",
  "appleIdentifier": "String",
  "topicIdentifier": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "certificate": "String"
}
```



