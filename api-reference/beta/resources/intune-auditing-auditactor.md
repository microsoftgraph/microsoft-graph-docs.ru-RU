---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc0af6bd60eae7a21b38905d4ea56e9ae7d70499
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792956"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="46462-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="46462-103">auditActor resource type</span></span>

<span data-ttu-id="46462-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46462-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46462-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46462-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="46462-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="46462-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46462-107">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="46462-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="46462-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="46462-108">Properties</span></span>
|<span data-ttu-id="46462-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="46462-109">Property</span></span>|<span data-ttu-id="46462-110">Тип</span><span class="sxs-lookup"><span data-stu-id="46462-110">Type</span></span>|<span data-ttu-id="46462-111">Описание</span><span class="sxs-lookup"><span data-stu-id="46462-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46462-112">type</span><span class="sxs-lookup"><span data-stu-id="46462-112">type</span></span>|<span data-ttu-id="46462-113">String</span><span class="sxs-lookup"><span data-stu-id="46462-113">String</span></span>|<span data-ttu-id="46462-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="46462-114">Actor Type.</span></span>|
|<span data-ttu-id="46462-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="46462-115">userPermissions</span></span>|<span data-ttu-id="46462-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="46462-116">String collection</span></span>|<span data-ttu-id="46462-117">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="46462-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="46462-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="46462-118">applicationId</span></span>|<span data-ttu-id="46462-119">String</span><span class="sxs-lookup"><span data-stu-id="46462-119">String</span></span>|<span data-ttu-id="46462-120">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="46462-120">AAD Application Id.</span></span>|
|<span data-ttu-id="46462-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="46462-121">applicationDisplayName</span></span>|<span data-ttu-id="46462-122">String</span><span class="sxs-lookup"><span data-stu-id="46462-122">String</span></span>|<span data-ttu-id="46462-123">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="46462-123">Name of the Application.</span></span>|
|<span data-ttu-id="46462-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="46462-124">userPrincipalName</span></span>|<span data-ttu-id="46462-125">String</span><span class="sxs-lookup"><span data-stu-id="46462-125">String</span></span>|<span data-ttu-id="46462-126">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="46462-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="46462-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="46462-127">servicePrincipalName</span></span>|<span data-ttu-id="46462-128">String</span><span class="sxs-lookup"><span data-stu-id="46462-128">String</span></span>|<span data-ttu-id="46462-129">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="46462-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="46462-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="46462-130">ipAddress</span></span>|<span data-ttu-id="46462-131">String</span><span class="sxs-lookup"><span data-stu-id="46462-131">String</span></span>|<span data-ttu-id="46462-132">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="46462-132">IPAddress.</span></span>|
|<span data-ttu-id="46462-133">userId</span><span class="sxs-lookup"><span data-stu-id="46462-133">userId</span></span>|<span data-ttu-id="46462-134">String</span><span class="sxs-lookup"><span data-stu-id="46462-134">String</span></span>|<span data-ttu-id="46462-135">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="46462-135">User Id.</span></span>|
|<span data-ttu-id="46462-136">усерролескопетагс</span><span class="sxs-lookup"><span data-stu-id="46462-136">userRoleScopeTags</span></span>|<span data-ttu-id="46462-137">Коллекция [ролескопетагинфо](../resources/intune-auditing-rolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="46462-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="46462-138">Список тегов области пользователя при выполнении аудита.</span><span class="sxs-lookup"><span data-stu-id="46462-138">List of user scope tags when the audit was performed.</span></span>|
|<span data-ttu-id="46462-139">ремотетенантид</span><span class="sxs-lookup"><span data-stu-id="46462-139">remoteTenantId</span></span>|<span data-ttu-id="46462-140">String</span><span class="sxs-lookup"><span data-stu-id="46462-140">String</span></span>|<span data-ttu-id="46462-141">Идентификатор удаленного клиента</span><span class="sxs-lookup"><span data-stu-id="46462-141">Remote Tenant Id</span></span>|
|<span data-ttu-id="46462-142">ремотеусерид</span><span class="sxs-lookup"><span data-stu-id="46462-142">remoteUserId</span></span>|<span data-ttu-id="46462-143">String</span><span class="sxs-lookup"><span data-stu-id="46462-143">String</span></span>|<span data-ttu-id="46462-144">Идентификатор удаленного пользователя</span><span class="sxs-lookup"><span data-stu-id="46462-144">Remote User Id</span></span>|

## <a name="relationships"></a><span data-ttu-id="46462-145">Связи</span><span class="sxs-lookup"><span data-stu-id="46462-145">Relationships</span></span>
<span data-ttu-id="46462-146">Нет</span><span class="sxs-lookup"><span data-stu-id="46462-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="46462-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="46462-147">JSON Representation</span></span>
<span data-ttu-id="46462-148">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="46462-148">Here is a JSON representation of the resource.</span></span>
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



