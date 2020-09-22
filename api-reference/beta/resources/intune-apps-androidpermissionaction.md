---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f053a3fa560bce29d0fe4aa66bb796b114658929
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004027"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="6fbca-103">Тип ресурса Андроидпермиссионактион</span><span class="sxs-lookup"><span data-stu-id="6fbca-103">androidPermissionAction resource type</span></span>

<span data-ttu-id="6fbca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fbca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6fbca-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6fbca-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6fbca-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6fbca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6fbca-107">Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.</span><span class="sxs-lookup"><span data-stu-id="6fbca-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="6fbca-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fbca-108">Properties</span></span>
|<span data-ttu-id="6fbca-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fbca-109">Property</span></span>|<span data-ttu-id="6fbca-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6fbca-110">Type</span></span>|<span data-ttu-id="6fbca-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6fbca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fbca-112">права</span><span class="sxs-lookup"><span data-stu-id="6fbca-112">permission</span></span>|<span data-ttu-id="6fbca-113">String</span><span class="sxs-lookup"><span data-stu-id="6fbca-113">String</span></span>|<span data-ttu-id="6fbca-114">Строка разрешений Android, определенная в официальной документации по Android.</span><span class="sxs-lookup"><span data-stu-id="6fbca-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="6fbca-115">Пример: "Android. Permission. READ_CONTACTS".</span><span class="sxs-lookup"><span data-stu-id="6fbca-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="6fbca-116">action</span><span class="sxs-lookup"><span data-stu-id="6fbca-116">action</span></span>|[<span data-ttu-id="6fbca-117">андроидпермиссионактионтипе</span><span class="sxs-lookup"><span data-stu-id="6fbca-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="6fbca-118">Тип действия разрешений Android.</span><span class="sxs-lookup"><span data-stu-id="6fbca-118">Type of Android permission action.</span></span> <span data-ttu-id="6fbca-119">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="6fbca-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fbca-120">Связи</span><span class="sxs-lookup"><span data-stu-id="6fbca-120">Relationships</span></span>
<span data-ttu-id="6fbca-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6fbca-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fbca-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fbca-122">JSON Representation</span></span>
<span data-ttu-id="6fbca-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fbca-123">Here is a JSON representation of the resource.</span></span>
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






