# <a name="rolepermission-resource-type"></a><span data-ttu-id="59d03-101">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="59d03-101">rolePermission resource type</span></span>

> <span data-ttu-id="59d03-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="59d03-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59d03-103">Н/Д</span><span class="sxs-lookup"><span data-stu-id="59d03-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="59d03-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="59d03-104">Properties</span></span>
|<span data-ttu-id="59d03-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="59d03-105">Property</span></span>|<span data-ttu-id="59d03-106">Тип</span><span class="sxs-lookup"><span data-stu-id="59d03-106">Type</span></span>|<span data-ttu-id="59d03-107">Описание</span><span class="sxs-lookup"><span data-stu-id="59d03-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59d03-108">resourceActions</span><span class="sxs-lookup"><span data-stu-id="59d03-108">resourceActions</span></span>|<span data-ttu-id="59d03-109">Коллекция объектов [resourceAction](../resources/intune_rbac_resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="59d03-109">[resourceAction](../resources/intune_rbac_resourceaction.md) collection</span></span>|<span data-ttu-id="59d03-110">Действия</span><span class="sxs-lookup"><span data-stu-id="59d03-110">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="59d03-111">Связи</span><span class="sxs-lookup"><span data-stu-id="59d03-111">Relationships</span></span>
<span data-ttu-id="59d03-112">Нет</span><span class="sxs-lookup"><span data-stu-id="59d03-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59d03-113">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="59d03-113">JSON Representation</span></span>
<span data-ttu-id="59d03-114">Ниже этот ресурс представлен в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="59d03-114">Here is a JSON representation of the resource.</span></span>
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



