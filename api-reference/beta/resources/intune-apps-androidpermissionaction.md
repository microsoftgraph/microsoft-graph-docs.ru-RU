---
title: Тип ресурса androidPermissionAction
description: Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: daf72bbc5f8d1e32480adeda72c3f759255f54db
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860538"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="2c227-103">Тип ресурса androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="2c227-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="2c227-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2c227-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2c227-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2c227-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2c227-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2c227-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2c227-107">Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.</span><span class="sxs-lookup"><span data-stu-id="2c227-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>
## <a name="properties"></a><span data-ttu-id="2c227-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c227-108">Properties</span></span>
|<span data-ttu-id="2c227-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c227-109">Property</span></span>|<span data-ttu-id="2c227-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2c227-110">Type</span></span>|<span data-ttu-id="2c227-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2c227-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c227-112">разрешение</span><span class="sxs-lookup"><span data-stu-id="2c227-112">permission</span></span>|<span data-ttu-id="2c227-113">Строка</span><span class="sxs-lookup"><span data-stu-id="2c227-113">String</span></span>|<span data-ttu-id="2c227-114">Строка, Android разрешений, определенных в Официальная документация Android.</span><span class="sxs-lookup"><span data-stu-id="2c227-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="2c227-115">Пример «android.permission.READ_CONTACTS».</span><span class="sxs-lookup"><span data-stu-id="2c227-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="2c227-116">action</span><span class="sxs-lookup"><span data-stu-id="2c227-116">action</span></span>|[<span data-ttu-id="2c227-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="2c227-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="2c227-118">Тип действия Android разрешений.</span><span class="sxs-lookup"><span data-stu-id="2c227-118">Type of Android permission action.</span></span> <span data-ttu-id="2c227-119">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="2c227-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c227-120">Связи</span><span class="sxs-lookup"><span data-stu-id="2c227-120">Relationships</span></span>
<span data-ttu-id="2c227-121">Нет</span><span class="sxs-lookup"><span data-stu-id="2c227-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2c227-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c227-122">JSON Representation</span></span>
<span data-ttu-id="2c227-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c227-123">Here is a JSON representation of the resource.</span></span>
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





