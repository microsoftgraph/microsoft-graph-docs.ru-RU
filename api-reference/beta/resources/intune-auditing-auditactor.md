---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 173afc06c20e01406172cf2bc6b8c785aac55aa9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403205"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="b1a86-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="b1a86-103">auditActor resource type</span></span>

<span data-ttu-id="b1a86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1a86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1a86-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1a86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1a86-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1a86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1a86-107">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="b1a86-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="b1a86-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1a86-108">Properties</span></span>
|<span data-ttu-id="b1a86-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1a86-109">Property</span></span>|<span data-ttu-id="b1a86-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b1a86-110">Type</span></span>|<span data-ttu-id="b1a86-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b1a86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a86-112">type</span><span class="sxs-lookup"><span data-stu-id="b1a86-112">type</span></span>|<span data-ttu-id="b1a86-113">String</span><span class="sxs-lookup"><span data-stu-id="b1a86-113">String</span></span>|<span data-ttu-id="b1a86-114">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="b1a86-114">Actor Type.</span></span>|
|<span data-ttu-id="b1a86-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="b1a86-115">userPermissions</span></span>|<span data-ttu-id="b1a86-116">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b1a86-116">String collection</span></span>|<span data-ttu-id="b1a86-117">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="b1a86-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="b1a86-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="b1a86-118">applicationId</span></span>|<span data-ttu-id="b1a86-119">String</span><span class="sxs-lookup"><span data-stu-id="b1a86-119">String</span></span>|<span data-ttu-id="b1a86-120">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="b1a86-120">AAD Application Id.</span></span>|
|<span data-ttu-id="b1a86-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b1a86-121">applicationDisplayName</span></span>|<span data-ttu-id="b1a86-122">String</span><span class="sxs-lookup"><span data-stu-id="b1a86-122">String</span></span>|<span data-ttu-id="b1a86-123">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="b1a86-123">Name of the Application.</span></span>|
|<span data-ttu-id="b1a86-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1a86-124">userPrincipalName</span></span>|<span data-ttu-id="b1a86-125">Строка</span><span class="sxs-lookup"><span data-stu-id="b1a86-125">String</span></span>|<span data-ttu-id="b1a86-126">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="b1a86-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="b1a86-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="b1a86-127">servicePrincipalName</span></span>|<span data-ttu-id="b1a86-128">String</span><span class="sxs-lookup"><span data-stu-id="b1a86-128">String</span></span>|<span data-ttu-id="b1a86-129">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="b1a86-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="b1a86-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b1a86-130">ipAddress</span></span>|<span data-ttu-id="b1a86-131">String</span><span class="sxs-lookup"><span data-stu-id="b1a86-131">String</span></span>|<span data-ttu-id="b1a86-132">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="b1a86-132">IPAddress.</span></span>|
|<span data-ttu-id="b1a86-133">userId</span><span class="sxs-lookup"><span data-stu-id="b1a86-133">userId</span></span>|<span data-ttu-id="b1a86-134">String</span><span class="sxs-lookup"><span data-stu-id="b1a86-134">String</span></span>|<span data-ttu-id="b1a86-135">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="b1a86-135">User Id.</span></span>|
|<span data-ttu-id="b1a86-136">усерролескопетагс</span><span class="sxs-lookup"><span data-stu-id="b1a86-136">userRoleScopeTags</span></span>|<span data-ttu-id="b1a86-137">Коллекция [ролескопетагинфо](../resources/intune-auditing-rolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="b1a86-137">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="b1a86-138">Список тегов области пользователя при выполнении аудита.</span><span class="sxs-lookup"><span data-stu-id="b1a86-138">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1a86-139">Связи</span><span class="sxs-lookup"><span data-stu-id="b1a86-139">Relationships</span></span>
<span data-ttu-id="b1a86-140">Нет</span><span class="sxs-lookup"><span data-stu-id="b1a86-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1a86-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1a86-141">JSON Representation</span></span>
<span data-ttu-id="b1a86-142">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1a86-142">Here is a JSON representation of the resource.</span></span>
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
  ]
}
```



