---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4766bb91d5d1cde99a12f5a8e4903451a3ac5aca
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950489"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="c275d-103">Тип ресурса Андроидпермиссионактион</span><span class="sxs-lookup"><span data-stu-id="c275d-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="c275d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c275d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c275d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c275d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c275d-106">Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.</span><span class="sxs-lookup"><span data-stu-id="c275d-106">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="c275d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c275d-107">Properties</span></span>
|<span data-ttu-id="c275d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c275d-108">Property</span></span>|<span data-ttu-id="c275d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c275d-109">Type</span></span>|<span data-ttu-id="c275d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c275d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c275d-111">права</span><span class="sxs-lookup"><span data-stu-id="c275d-111">permission</span></span>|<span data-ttu-id="c275d-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c275d-112">String</span></span>|<span data-ttu-id="c275d-113">Строка разрешений Android, определенная в официальной документации по Android.</span><span class="sxs-lookup"><span data-stu-id="c275d-113">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="c275d-114">Пример: "Android. Permission. РЕАД_КОНТАКТС".</span><span class="sxs-lookup"><span data-stu-id="c275d-114">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="c275d-115">action</span><span class="sxs-lookup"><span data-stu-id="c275d-115">action</span></span>|[<span data-ttu-id="c275d-116">Андроидпермиссионактионтипе</span><span class="sxs-lookup"><span data-stu-id="c275d-116">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="c275d-117">Тип действия разрешений Android.</span><span class="sxs-lookup"><span data-stu-id="c275d-117">Type of Android permission action.</span></span> <span data-ttu-id="c275d-118">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="c275d-118">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c275d-119">Связи</span><span class="sxs-lookup"><span data-stu-id="c275d-119">Relationships</span></span>
<span data-ttu-id="c275d-120">Нет</span><span class="sxs-lookup"><span data-stu-id="c275d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c275d-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c275d-121">JSON Representation</span></span>
<span data-ttu-id="c275d-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c275d-122">Here is a JSON representation of the resource.</span></span>
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




