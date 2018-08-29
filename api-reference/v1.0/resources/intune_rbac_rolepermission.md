# <a name="rolepermission-resource-type"></a><span data-ttu-id="dfe93-101">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="dfe93-101">rolePermission resource type</span></span>

> <span data-ttu-id="dfe93-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="dfe93-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfe93-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="dfe93-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="dfe93-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="dfe93-104">Properties</span></span>
|<span data-ttu-id="dfe93-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="dfe93-105">Property</span></span>|<span data-ttu-id="dfe93-106">Тип</span><span class="sxs-lookup"><span data-stu-id="dfe93-106">Type</span></span>|<span data-ttu-id="dfe93-107">Описание</span><span class="sxs-lookup"><span data-stu-id="dfe93-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfe93-108">resourceActions</span><span class="sxs-lookup"><span data-stu-id="dfe93-108">resourceActions</span></span>|<span data-ttu-id="dfe93-109">Коллекция объектов [resourceAction](../resources/intune_rbac_resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="dfe93-109">[resourceAction](../resources/intune_rbac_resourceaction.md) collection</span></span>|<span data-ttu-id="dfe93-110">Действия</span><span class="sxs-lookup"><span data-stu-id="dfe93-110">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfe93-111">Связи</span><span class="sxs-lookup"><span data-stu-id="dfe93-111">Relationships</span></span>
<span data-ttu-id="dfe93-112">Нет</span><span class="sxs-lookup"><span data-stu-id="dfe93-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dfe93-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dfe93-113">JSON Representation</span></span>
<span data-ttu-id="dfe93-114">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dfe93-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```



