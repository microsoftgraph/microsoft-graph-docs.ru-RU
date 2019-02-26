---
title: Тип ресурса rolePermission
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b56df927cda3cbf98e7d736311aba2db5e53906
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145383"
---
# <a name="rolepermission-resource-type"></a><span data-ttu-id="2cb57-103">Тип ресурса rolePermission</span><span class="sxs-lookup"><span data-stu-id="2cb57-103">rolePermission resource type</span></span>

> <span data-ttu-id="2cb57-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2cb57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cb57-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2cb57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cb57-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="2cb57-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2cb57-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2cb57-107">Properties</span></span>
|<span data-ttu-id="2cb57-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2cb57-108">Property</span></span>|<span data-ttu-id="2cb57-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2cb57-109">Type</span></span>|<span data-ttu-id="2cb57-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2cb57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cb57-111">actions</span><span class="sxs-lookup"><span data-stu-id="2cb57-111">actions</span></span>|<span data-ttu-id="2cb57-112">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="2cb57-112">String collection</span></span>|<span data-ttu-id="2cb57-113">Разрешенные действия</span><span class="sxs-lookup"><span data-stu-id="2cb57-113">Allowed Actions</span></span>|
|<span data-ttu-id="2cb57-114">resourceActions</span><span class="sxs-lookup"><span data-stu-id="2cb57-114">resourceActions</span></span>|<span data-ttu-id="2cb57-115">Коллекция объектов [resourceAction](../resources/intune-rbac-resourceaction.md)</span><span class="sxs-lookup"><span data-stu-id="2cb57-115">[resourceAction](../resources/intune-rbac-resourceaction.md) collection</span></span>|<span data-ttu-id="2cb57-116">Действия</span><span class="sxs-lookup"><span data-stu-id="2cb57-116">Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cb57-117">Связи</span><span class="sxs-lookup"><span data-stu-id="2cb57-117">Relationships</span></span>
<span data-ttu-id="2cb57-118">Нет</span><span class="sxs-lookup"><span data-stu-id="2cb57-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cb57-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2cb57-119">JSON Representation</span></span>
<span data-ttu-id="2cb57-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2cb57-120">Here is a JSON representation of the resource.</span></span>
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




