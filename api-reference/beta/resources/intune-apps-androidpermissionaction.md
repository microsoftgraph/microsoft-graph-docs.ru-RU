---
title: Тип ресурса androidPermissionAction
description: Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 62355c3427083df09963e316f3b6b3c104a8662f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425633"
---
# <a name="androidpermissionaction-resource-type"></a><span data-ttu-id="44b0d-103">Тип ресурса androidPermissionAction</span><span class="sxs-lookup"><span data-stu-id="44b0d-103">androidPermissionAction resource type</span></span>

> <span data-ttu-id="44b0d-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="44b0d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="44b0d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="44b0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44b0d-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44b0d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44b0d-107">Сопоставление разрешений для Android и Android действие должен выполнять при запросе это разрешение.</span><span class="sxs-lookup"><span data-stu-id="44b0d-107">Mapping between an Android app permission and the action Android should take when that permission is requested.</span></span>

## <a name="properties"></a><span data-ttu-id="44b0d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="44b0d-108">Properties</span></span>
|<span data-ttu-id="44b0d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="44b0d-109">Property</span></span>|<span data-ttu-id="44b0d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="44b0d-110">Type</span></span>|<span data-ttu-id="44b0d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="44b0d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44b0d-112">разрешение</span><span class="sxs-lookup"><span data-stu-id="44b0d-112">permission</span></span>|<span data-ttu-id="44b0d-113">String</span><span class="sxs-lookup"><span data-stu-id="44b0d-113">String</span></span>|<span data-ttu-id="44b0d-114">Строка, Android разрешений, определенных в Официальная документация Android.</span><span class="sxs-lookup"><span data-stu-id="44b0d-114">Android permission string, defined in the official Android documentation.</span></span>  <span data-ttu-id="44b0d-115">Пример «android.permission.READ_CONTACTS».</span><span class="sxs-lookup"><span data-stu-id="44b0d-115">Example 'android.permission.READ_CONTACTS'.</span></span>|
|<span data-ttu-id="44b0d-116">action</span><span class="sxs-lookup"><span data-stu-id="44b0d-116">action</span></span>|[<span data-ttu-id="44b0d-117">androidPermissionActionType</span><span class="sxs-lookup"><span data-stu-id="44b0d-117">androidPermissionActionType</span></span>](../resources/intune-apps-androidpermissionactiontype.md)|<span data-ttu-id="44b0d-118">Тип действия Android разрешений.</span><span class="sxs-lookup"><span data-stu-id="44b0d-118">Type of Android permission action.</span></span> <span data-ttu-id="44b0d-119">Возможные значения: `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="44b0d-119">Possible values are: `prompt`, `autoGrant`, `autoDeny`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44b0d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="44b0d-120">Relationships</span></span>
<span data-ttu-id="44b0d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="44b0d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44b0d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44b0d-122">JSON Representation</span></span>
<span data-ttu-id="44b0d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44b0d-123">Here is a JSON representation of the resource.</span></span>
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




