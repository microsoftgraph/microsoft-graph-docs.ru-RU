---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce351edc83ac31c21c05b7d3e64c2f3be315da61
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42799264"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="6a046-103">Тип ресурса Андроидпермиссионактион</span><span class="sxs-lookup"><span data-stu-id="6a046-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="6a046-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a046-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a046-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a046-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a046-106">Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.</span><span class="sxs-lookup"><span data-stu-id="6a046-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="6a046-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a046-107">Properties</span></span>
|<span data-ttu-id="6a046-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a046-108">Property</span></span>|<span data-ttu-id="6a046-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6a046-109">Type</span></span>|<span data-ttu-id="6a046-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a046-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a046-111">права</span><span class="sxs-lookup"><span data-stu-id="6a046-111">permission</span></span>|<span data-ttu-id="6a046-112">String</span><span class="sxs-lookup"><span data-stu-id="6a046-112">String</span></span>|<span data-ttu-id="6a046-113">Строка разрешений Android, определенная в официальной документации по Android.</span><span class="sxs-lookup"><span data-stu-id="6a046-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="6a046-114">Пример: "Android. Permission. READ_CONTACTS".</span><span class="sxs-lookup"><span data-stu-id="6a046-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="6a046-115">action</span><span class="sxs-lookup"><span data-stu-id="6a046-115">action</span></span>|[<span data-ttu-id="6a046-116">андроидпермиссионактионтипе</span><span class="sxs-lookup"><span data-stu-id="6a046-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="6a046-117">Тип действия разрешений Android.</span><span class="sxs-lookup"><span data-stu-id="6a046-117">Type of Android permission action.</span></span> <span data-ttu-id="6a046-118">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="6a046-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a046-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6a046-119">Relationships</span></span>
<span data-ttu-id="6a046-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6a046-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a046-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a046-121">JSON Representation</span></span>
<span data-ttu-id="6a046-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a046-122">Here is a JSON representation of the resource.</span></span>
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



