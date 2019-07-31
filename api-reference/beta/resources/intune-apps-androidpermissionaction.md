---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ca8511f584ae0fe69ee558d4808e333d57259142
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006096"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="e8074-103">Тип ресурса Андроидпермиссионактион</span><span class="sxs-lookup"><span data-stu-id="e8074-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="e8074-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8074-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8074-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8074-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8074-106">Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.</span><span class="sxs-lookup"><span data-stu-id="e8074-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="e8074-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8074-107">Properties</span></span>
|<span data-ttu-id="e8074-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8074-108">Property</span></span>|<span data-ttu-id="e8074-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e8074-109">Type</span></span>|<span data-ttu-id="e8074-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e8074-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8074-111">permission</span><span class="sxs-lookup"><span data-stu-id="e8074-111">permission</span></span>|<span data-ttu-id="e8074-112">String</span><span class="sxs-lookup"><span data-stu-id="e8074-112">String</span></span>|<span data-ttu-id="e8074-113">Строка разрешений Android, определенная в официальной документации по Android.</span><span class="sxs-lookup"><span data-stu-id="e8074-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="e8074-114">Пример: "Android. Permission. РЕАД_КОНТАКТС".</span><span class="sxs-lookup"><span data-stu-id="e8074-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="e8074-115">action</span><span class="sxs-lookup"><span data-stu-id="e8074-115">action</span></span>|[<span data-ttu-id="e8074-116">Андроидпермиссионактионтипе</span><span class="sxs-lookup"><span data-stu-id="e8074-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="e8074-117">Тип действия разрешений Android.</span><span class="sxs-lookup"><span data-stu-id="e8074-117">Type of Android permission action.</span></span> <span data-ttu-id="e8074-118">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="e8074-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8074-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="e8074-119">Relationships</span></span>
<span data-ttu-id="e8074-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e8074-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8074-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8074-121">JSON Representation</span></span>
<span data-ttu-id="e8074-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8074-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```





