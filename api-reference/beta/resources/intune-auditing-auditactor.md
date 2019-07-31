---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb27d70155716e0e30b80c5f9fa7c77b0386b011
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004892"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="bc8b8-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="bc8b8-103">auditActor resource type</span></span>

> <span data-ttu-id="bc8b8-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc8b8-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc8b8-106">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="bc8b8-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc8b8-107">Properties</span></span>
|<span data-ttu-id="bc8b8-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc8b8-108">Property</span></span>|<span data-ttu-id="bc8b8-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bc8b8-109">Type</span></span>|<span data-ttu-id="bc8b8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc8b8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc8b8-111">type</span><span class="sxs-lookup"><span data-stu-id="bc8b8-111">type</span></span>|<span data-ttu-id="bc8b8-112">String</span><span class="sxs-lookup"><span data-stu-id="bc8b8-112">String</span></span>|<span data-ttu-id="bc8b8-113">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-113">Actor Type.</span></span>|
|<span data-ttu-id="bc8b8-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="bc8b8-114">userPermissions</span></span>|<span data-ttu-id="bc8b8-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="bc8b8-115">String collection</span></span>|<span data-ttu-id="bc8b8-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="bc8b8-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="bc8b8-117">applicationId</span></span>|<span data-ttu-id="bc8b8-118">String</span><span class="sxs-lookup"><span data-stu-id="bc8b8-118">String</span></span>|<span data-ttu-id="bc8b8-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-119">AAD Application Id.</span></span>|
|<span data-ttu-id="bc8b8-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="bc8b8-120">applicationDisplayName</span></span>|<span data-ttu-id="bc8b8-121">String</span><span class="sxs-lookup"><span data-stu-id="bc8b8-121">String</span></span>|<span data-ttu-id="bc8b8-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-122">Name of the Application.</span></span>|
|<span data-ttu-id="bc8b8-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc8b8-123">userPrincipalName</span></span>|<span data-ttu-id="bc8b8-124">Строка</span><span class="sxs-lookup"><span data-stu-id="bc8b8-124">String</span></span>|<span data-ttu-id="bc8b8-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="bc8b8-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="bc8b8-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="bc8b8-126">servicePrincipalName</span></span>|<span data-ttu-id="bc8b8-127">String</span><span class="sxs-lookup"><span data-stu-id="bc8b8-127">String</span></span>|<span data-ttu-id="bc8b8-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="bc8b8-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="bc8b8-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="bc8b8-129">ipAddress</span></span>|<span data-ttu-id="bc8b8-130">String</span><span class="sxs-lookup"><span data-stu-id="bc8b8-130">String</span></span>|<span data-ttu-id="bc8b8-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-131">IPAddress.</span></span>|
|<span data-ttu-id="bc8b8-132">userId</span><span class="sxs-lookup"><span data-stu-id="bc8b8-132">userId</span></span>|<span data-ttu-id="bc8b8-133">String</span><span class="sxs-lookup"><span data-stu-id="bc8b8-133">String</span></span>|<span data-ttu-id="bc8b8-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc8b8-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="bc8b8-135">Relationships</span></span>
<span data-ttu-id="bc8b8-136">Нет</span><span class="sxs-lookup"><span data-stu-id="bc8b8-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc8b8-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc8b8-137">JSON Representation</span></span>
<span data-ttu-id="bc8b8-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc8b8-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```





