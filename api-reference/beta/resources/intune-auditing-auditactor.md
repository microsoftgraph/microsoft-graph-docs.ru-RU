---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fd8edf9b9ab9b0513e77bbef6ce04dfcd5d4a1a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48019567"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="7bbeb-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="7bbeb-103">auditActor resource type</span></span>

<span data-ttu-id="7bbeb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bbeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bbeb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bbeb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bbeb-107">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="7bbeb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7bbeb-108">Properties</span></span>
|<span data-ttu-id="7bbeb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7bbeb-109">Property</span></span>|<span data-ttu-id="7bbeb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7bbeb-110">Type</span></span>|<span data-ttu-id="7bbeb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7bbeb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bbeb-112">type</span><span class="sxs-lookup"><span data-stu-id="7bbeb-112">type</span></span>|<span data-ttu-id="7bbeb-113">String</span><span class="sxs-lookup"><span data-stu-id="7bbeb-113">String</span></span>|<span data-ttu-id="7bbeb-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-114">Actor Type.</span></span>|
|<span data-ttu-id="7bbeb-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="7bbeb-115">userPermissions</span></span>|<span data-ttu-id="7bbeb-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="7bbeb-116">String collection</span></span>|<span data-ttu-id="7bbeb-117">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="7bbeb-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="7bbeb-118">applicationId</span></span>|<span data-ttu-id="7bbeb-119">String</span><span class="sxs-lookup"><span data-stu-id="7bbeb-119">String</span></span>|<span data-ttu-id="7bbeb-120">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-120">AAD Application Id.</span></span>|
|<span data-ttu-id="7bbeb-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="7bbeb-121">applicationDisplayName</span></span>|<span data-ttu-id="7bbeb-122">String</span><span class="sxs-lookup"><span data-stu-id="7bbeb-122">String</span></span>|<span data-ttu-id="7bbeb-123">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-123">Name of the Application.</span></span>|
|<span data-ttu-id="7bbeb-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7bbeb-124">userPrincipalName</span></span>|<span data-ttu-id="7bbeb-125">String</span><span class="sxs-lookup"><span data-stu-id="7bbeb-125">String</span></span>|<span data-ttu-id="7bbeb-126">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="7bbeb-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="7bbeb-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="7bbeb-127">servicePrincipalName</span></span>|<span data-ttu-id="7bbeb-128">String</span><span class="sxs-lookup"><span data-stu-id="7bbeb-128">String</span></span>|<span data-ttu-id="7bbeb-129">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="7bbeb-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="7bbeb-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="7bbeb-130">ipAddress</span></span>|<span data-ttu-id="7bbeb-131">String</span><span class="sxs-lookup"><span data-stu-id="7bbeb-131">String</span></span>|<span data-ttu-id="7bbeb-132">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-132">IPAddress.</span></span>|
|<span data-ttu-id="7bbeb-133">userId</span><span class="sxs-lookup"><span data-stu-id="7bbeb-133">userId</span></span>|<span data-ttu-id="7bbeb-134">String</span><span class="sxs-lookup"><span data-stu-id="7bbeb-134">String</span></span>|<span data-ttu-id="7bbeb-135">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-135">User Id.</span></span>|
|<span data-ttu-id="7bbeb-136">усерролескопетагс</span><span class="sxs-lookup"><span data-stu-id="7bbeb-136">userRoleScopeTags</span></span>|<span data-ttu-id="7bbeb-137">Коллекция [ролескопетагинфо](../resources/intune-auditing-rolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="7bbeb-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="7bbeb-138">Список тегов области пользователя при выполнении аудита.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-138">List of user scope tags when the audit was performed.</span></span>|
|<span data-ttu-id="7bbeb-139">ремотетенантид</span><span class="sxs-lookup"><span data-stu-id="7bbeb-139">remoteTenantId</span></span>|<span data-ttu-id="7bbeb-140">String</span><span class="sxs-lookup"><span data-stu-id="7bbeb-140">String</span></span>|<span data-ttu-id="7bbeb-141">Идентификатор удаленного клиента</span><span class="sxs-lookup"><span data-stu-id="7bbeb-141">Remote Tenant Id</span></span>|
|<span data-ttu-id="7bbeb-142">ремотеусерид</span><span class="sxs-lookup"><span data-stu-id="7bbeb-142">remoteUserId</span></span>|<span data-ttu-id="7bbeb-143">String</span><span class="sxs-lookup"><span data-stu-id="7bbeb-143">String</span></span>|<span data-ttu-id="7bbeb-144">Идентификатор удаленного пользователя</span><span class="sxs-lookup"><span data-stu-id="7bbeb-144">Remote User Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bbeb-145">Отношения</span><span class="sxs-lookup"><span data-stu-id="7bbeb-145">Relationships</span></span>
<span data-ttu-id="7bbeb-146">Нет</span><span class="sxs-lookup"><span data-stu-id="7bbeb-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bbeb-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7bbeb-147">JSON Representation</span></span>
<span data-ttu-id="7bbeb-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7bbeb-148">Here is a JSON representation of the resource.</span></span>
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
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.roleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ],
  "remoteTenantId": "String",
  "remoteUserId": "String"
}
```






