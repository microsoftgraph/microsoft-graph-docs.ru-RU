---
title: Тип ресурса androidPermissionAction
description: Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
author: tfitzmac
ms.openlocfilehash: 90117b30dae765151e79d8ad1c2ae1afaa5a42ff
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331138"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="c969c-103">Тип ресурса androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="c969c-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="c969c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c969c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c969c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c969c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c969c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c969c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c969c-107">Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.</span><span class="sxs-lookup"><span data-stu-id="c969c-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>
## <a name="properties"></a><span data-ttu-id="c969c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c969c-108">Properties</span></span>
|<span data-ttu-id="c969c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c969c-109">Property</span></span>|<span data-ttu-id="c969c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c969c-110">Type</span></span>|<span data-ttu-id="c969c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c969c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c969c-112">разрешение</span><span class="sxs-lookup"><span data-stu-id="c969c-112">permission</span></span>|<span data-ttu-id="c969c-113">String.</span><span class="sxs-lookup"><span data-stu-id="c969c-113">String</span></span>|<span data-ttu-id="c969c-114">Строка, Android разрешений, определенных в Официальная документация Android.</span><span class="sxs-lookup"><span data-stu-id="c969c-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="c969c-115">Пример «android.permission.READ_CONTACTS».</span><span class="sxs-lookup"><span data-stu-id="c969c-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="c969c-116">action</span><span class="sxs-lookup"><span data-stu-id="c969c-116">action</span></span>|[<span data-ttu-id="c969c-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="c969c-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="c969c-118">Тип действия Android разрешений.</span><span class="sxs-lookup"><span data-stu-id="c969c-118">Type of Android permission action.</span></span> <span data-ttu-id="c969c-119">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="c969c-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c969c-120">Связи</span><span class="sxs-lookup"><span data-stu-id="c969c-120">Relationships</span></span>
<span data-ttu-id="c969c-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c969c-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c969c-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c969c-122">JSON Representation</span></span>
<span data-ttu-id="c969c-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c969c-123">Here is a JSON representation of the resource.</span></span>
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





