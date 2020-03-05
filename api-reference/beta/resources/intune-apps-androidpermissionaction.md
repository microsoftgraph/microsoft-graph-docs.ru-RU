---
title: Тип ресурса Андроидпермиссионактион
description: Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52b105c831399b935196254d794bd5da513d19f0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42494102"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="6e54d-103">Тип ресурса Андроидпермиссионактион</span><span class="sxs-lookup"><span data-stu-id="6e54d-103">androidPermissionAction resource type</span></span>

<span data-ttu-id="6e54d-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6e54d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e54d-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e54d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e54d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e54d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e54d-107">Сопоставление разрешений приложения Android и действия, выполняемого Android, должны выполняться при запросе этого разрешения.</span><span class="sxs-lookup"><span data-stu-id="6e54d-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="6e54d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e54d-108">Properties</span></span>
|<span data-ttu-id="6e54d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e54d-109">Property</span></span>|<span data-ttu-id="6e54d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6e54d-110">Type</span></span>|<span data-ttu-id="6e54d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6e54d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e54d-112">права</span><span class="sxs-lookup"><span data-stu-id="6e54d-112">permission</span></span>|<span data-ttu-id="6e54d-113">String</span><span class="sxs-lookup"><span data-stu-id="6e54d-113">String</span></span>|<span data-ttu-id="6e54d-114">Строка разрешений Android, определенная в официальной документации по Android.</span><span class="sxs-lookup"><span data-stu-id="6e54d-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="6e54d-115">Пример: "Android. Permission. READ_CONTACTS".</span><span class="sxs-lookup"><span data-stu-id="6e54d-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="6e54d-116">action</span><span class="sxs-lookup"><span data-stu-id="6e54d-116">action</span></span>|[<span data-ttu-id="6e54d-117">андроидпермиссионактионтипе</span><span class="sxs-lookup"><span data-stu-id="6e54d-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="6e54d-118">Тип действия разрешений Android.</span><span class="sxs-lookup"><span data-stu-id="6e54d-118">Type of Android permission action.</span></span> <span data-ttu-id="6e54d-119">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="6e54d-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e54d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="6e54d-120">Relationships</span></span>
<span data-ttu-id="6e54d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6e54d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e54d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e54d-122">JSON Representation</span></span>
<span data-ttu-id="6e54d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e54d-123">Here is a JSON representation of the resource.</span></span>
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



