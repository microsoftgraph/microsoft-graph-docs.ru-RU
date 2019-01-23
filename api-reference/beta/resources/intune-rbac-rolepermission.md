---
title: Тип ресурса rolePermission
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 932fff06ac979d6ec18ac4c79d50777552e8bfc7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395001"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="f10a0-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="f10a0-103">rolePermission resource type</span></span>

> <span data-ttu-id="f10a0-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f10a0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f10a0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f10a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f10a0-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f10a0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f10a0-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="f10a0-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f10a0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f10a0-108">Properties</span></span>
|<span data-ttu-id="f10a0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f10a0-109">Property</span></span>|<span data-ttu-id="f10a0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f10a0-110">Type</span></span>|<span data-ttu-id="f10a0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f10a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f10a0-112">actions</span><span class="sxs-lookup"><span data-stu-id="f10a0-112">actions</span></span>|<span data-ttu-id="f10a0-113">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f10a0-113">String collection</span></span>|<span data-ttu-id="f10a0-114">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="f10a0-114">Allowed Actions</span></span>|
|<span data-ttu-id="f10a0-115">resourceActions</span><span class="sxs-lookup"><span data-stu-id="f10a0-115">resourceActions</span></span>|<span data-ttu-id="f10a0-116">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="f10a0-116">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="f10a0-117">Действия</span><span class="sxs-lookup"><span data-stu-id="f10a0-117">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="f10a0-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f10a0-118">Relationships</span></span>
<span data-ttu-id="f10a0-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f10a0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f10a0-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f10a0-120">JSON Representation</span></span>
<span data-ttu-id="f10a0-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f10a0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rolePermission"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rolePermission",
  "actions": [
    "String"
  ],
  "resourceActions": [
    {
      "@odata.type": "microsoft.graph.resourceAction",
      "allowedResourceActions": [
        "String"
      ],
      "notAllowedResourceActions": [
        "String"
      ]
    }
  ]
}
```




