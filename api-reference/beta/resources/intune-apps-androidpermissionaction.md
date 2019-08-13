---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0d2aa07ae9064a6e7d04ea7e2f0dc07e06cfb627
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366891"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="6e83f-103">Тип ресурса Андроидпермиссионактион</span><span class="sxs-lookup"><span data-stu-id="6e83f-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="6e83f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e83f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e83f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e83f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e83f-106">Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.</span><span class="sxs-lookup"><span data-stu-id="6e83f-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="6e83f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e83f-107">Properties</span></span>
|<span data-ttu-id="6e83f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e83f-108">Property</span></span>|<span data-ttu-id="6e83f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e83f-109">Type</span></span>|<span data-ttu-id="6e83f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e83f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e83f-111">permission</span><span class="sxs-lookup"><span data-stu-id="6e83f-111">permission</span></span>|<span data-ttu-id="6e83f-112">String</span><span class="sxs-lookup"><span data-stu-id="6e83f-112">String</span></span>|<span data-ttu-id="6e83f-113">Строка разрешений Android, определенная в официальной документации по Android.</span><span class="sxs-lookup"><span data-stu-id="6e83f-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="6e83f-114">Пример: "Android. Permission. READ_CONTACTS".</span><span class="sxs-lookup"><span data-stu-id="6e83f-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="6e83f-115">action</span><span class="sxs-lookup"><span data-stu-id="6e83f-115">action</span></span>|[<span data-ttu-id="6e83f-116">андроидпермиссионактионтипе</span><span class="sxs-lookup"><span data-stu-id="6e83f-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="6e83f-117">Тип действия разрешений Android.</span><span class="sxs-lookup"><span data-stu-id="6e83f-117">Type of Android permission action.</span></span> <span data-ttu-id="6e83f-118">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="6e83f-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e83f-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="6e83f-119">Relationships</span></span>
<span data-ttu-id="6e83f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6e83f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e83f-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e83f-121">JSON Representation</span></span>
<span data-ttu-id="6e83f-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e83f-122">Here is a JSON representation of the resource.</span></span>
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



