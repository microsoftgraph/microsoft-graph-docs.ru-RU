# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="d24db-101">Тип ресурса managedAppPolicyDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="d24db-101">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="d24db-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d24db-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d24db-103">Представляет сводку по развертыванию политик для приложений.</span><span class="sxs-lookup"><span data-stu-id="d24db-103">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="d24db-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="d24db-104">Properties</span></span>
|<span data-ttu-id="d24db-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="d24db-105">Property</span></span>|<span data-ttu-id="d24db-106">Тип</span><span class="sxs-lookup"><span data-stu-id="d24db-106">Type</span></span>|<span data-ttu-id="d24db-107">Описание</span><span class="sxs-lookup"><span data-stu-id="d24db-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d24db-108">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d24db-108">mobileAppIdentifier</span></span>|[<span data-ttu-id="d24db-109">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d24db-109">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="d24db-110">Развертывание приложения.</span><span class="sxs-lookup"><span data-stu-id="d24db-110">Deployment of an app.</span></span>|
|<span data-ttu-id="d24db-111">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="d24db-111">configurationAppliedUserCount</span></span>|<span data-ttu-id="d24db-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d24db-112">Int32</span></span>|<span data-ttu-id="d24db-113">Количество пользователей, к которым применяется политика.</span><span class="sxs-lookup"><span data-stu-id="d24db-113">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d24db-114">Связи</span><span class="sxs-lookup"><span data-stu-id="d24db-114">Relationships</span></span>
<span data-ttu-id="d24db-115">Нет</span><span class="sxs-lookup"><span data-stu-id="d24db-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d24db-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d24db-116">JSON Representation</span></span>
<span data-ttu-id="d24db-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d24db-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```








