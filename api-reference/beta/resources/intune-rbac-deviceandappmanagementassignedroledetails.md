---
title: Тип ресурса deviceAndAppManagementAssignedRoleDetails
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d6ace16ba496feb24948c3e40c32dd8fcb2fcf48
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428916"
---
# <a name="deviceandappmanagementassignedroledetails-resource-type"></a><span data-ttu-id="0c91f-103">Тип ресурса deviceAndAppManagementAssignedRoleDetails</span><span class="sxs-lookup"><span data-stu-id="0c91f-103">deviceAndAppManagementAssignedRoleDetails resource type</span></span>

> <span data-ttu-id="0c91f-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0c91f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0c91f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c91f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c91f-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c91f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c91f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0c91f-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0c91f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0c91f-108">Properties</span></span>
|<span data-ttu-id="0c91f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0c91f-109">Property</span></span>|<span data-ttu-id="0c91f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0c91f-110">Type</span></span>|<span data-ttu-id="0c91f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c91f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c91f-112">roleDefinitionIds</span><span class="sxs-lookup"><span data-stu-id="0c91f-112">roleDefinitionIds</span></span>|<span data-ttu-id="0c91f-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0c91f-113">String collection</span></span>|<span data-ttu-id="0c91f-114">Идентификаторы определения ролей особую определения ролей, назначенных пользователю.</span><span class="sxs-lookup"><span data-stu-id="0c91f-114">Role Definition IDs for the specifc Role Definitions assigned to a user.</span></span>|
|<span data-ttu-id="0c91f-115">roleAssignmentIds</span><span class="sxs-lookup"><span data-stu-id="0c91f-115">roleAssignmentIds</span></span>|<span data-ttu-id="0c91f-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0c91f-116">String collection</span></span>|<span data-ttu-id="0c91f-117">Идентификаторы назначения ролей для назначения ролей, назначенных пользователю особую.</span><span class="sxs-lookup"><span data-stu-id="0c91f-117">Role Assignment IDs for the specifc Role Assignments assigned to a user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c91f-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="0c91f-118">Relationships</span></span>
<span data-ttu-id="0c91f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0c91f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c91f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0c91f-120">JSON Representation</span></span>
<span data-ttu-id="0c91f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0c91f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
  "roleDefinitionIds": [
    "String"
  ],
  "roleAssignmentIds": [
    "String"
  ]
}
```




