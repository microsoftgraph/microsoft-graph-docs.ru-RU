---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76090d450332b0c5656ee122a7338180fa692811
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231922"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="30bbb-103">Тип ресурса Андроидпермиссионактион</span><span class="sxs-lookup"><span data-stu-id="30bbb-103">androidPermissionAction resource type</span></span>

<span data-ttu-id="30bbb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30bbb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30bbb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30bbb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30bbb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="30bbb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30bbb-107">Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.</span><span class="sxs-lookup"><span data-stu-id="30bbb-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="30bbb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="30bbb-108">Properties</span></span>
|<span data-ttu-id="30bbb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="30bbb-109">Property</span></span>|<span data-ttu-id="30bbb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="30bbb-110">Type</span></span>|<span data-ttu-id="30bbb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="30bbb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30bbb-112">права</span><span class="sxs-lookup"><span data-stu-id="30bbb-112">permission</span></span>|<span data-ttu-id="30bbb-113">String</span><span class="sxs-lookup"><span data-stu-id="30bbb-113">String</span></span>|<span data-ttu-id="30bbb-114">Строка разрешений Android, определенная в официальной документации по Android.</span><span class="sxs-lookup"><span data-stu-id="30bbb-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="30bbb-115">Пример: "android.permission.READ_CONTACTS".</span><span class="sxs-lookup"><span data-stu-id="30bbb-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="30bbb-116">action</span><span class="sxs-lookup"><span data-stu-id="30bbb-116">action</span></span>|[<span data-ttu-id="30bbb-117">андроидпермиссионактионтипе</span><span class="sxs-lookup"><span data-stu-id="30bbb-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="30bbb-118">Тип действия разрешений Android.</span><span class="sxs-lookup"><span data-stu-id="30bbb-118">Type of Android permission action.</span></span> <span data-ttu-id="30bbb-119">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="30bbb-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30bbb-120">Связи</span><span class="sxs-lookup"><span data-stu-id="30bbb-120">Relationships</span></span>
<span data-ttu-id="30bbb-121">Нет</span><span class="sxs-lookup"><span data-stu-id="30bbb-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="30bbb-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="30bbb-122">JSON Representation</span></span>
<span data-ttu-id="30bbb-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="30bbb-123">Here is a JSON representation of the resource.</span></span>
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




