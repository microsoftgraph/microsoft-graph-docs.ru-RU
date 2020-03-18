---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1d54d34081c931df442afa6d6d0e569de75fb652
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797439"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="f1106-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="f1106-103">auditActor resource type</span></span>

> <span data-ttu-id="f1106-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1106-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f1106-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f1106-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f1106-106">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="f1106-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="f1106-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1106-107">Properties</span></span>
|<span data-ttu-id="f1106-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1106-108">Property</span></span>|<span data-ttu-id="f1106-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f1106-109">Type</span></span>|<span data-ttu-id="f1106-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f1106-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1106-111">type</span><span class="sxs-lookup"><span data-stu-id="f1106-111">type</span></span>|<span data-ttu-id="f1106-112">String</span><span class="sxs-lookup"><span data-stu-id="f1106-112">String</span></span>|<span data-ttu-id="f1106-113">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="f1106-113">Actor Type.</span></span>|
|<span data-ttu-id="f1106-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="f1106-114">userPermissions</span></span>|<span data-ttu-id="f1106-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f1106-115">String collection</span></span>|<span data-ttu-id="f1106-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="f1106-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="f1106-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="f1106-117">applicationId</span></span>|<span data-ttu-id="f1106-118">String</span><span class="sxs-lookup"><span data-stu-id="f1106-118">String</span></span>|<span data-ttu-id="f1106-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="f1106-119">AAD Application Id.</span></span>|
|<span data-ttu-id="f1106-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1106-120">applicationDisplayName</span></span>|<span data-ttu-id="f1106-121">String</span><span class="sxs-lookup"><span data-stu-id="f1106-121">String</span></span>|<span data-ttu-id="f1106-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="f1106-122">Name of the Application.</span></span>|
|<span data-ttu-id="f1106-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1106-123">userPrincipalName</span></span>|<span data-ttu-id="f1106-124">Строка</span><span class="sxs-lookup"><span data-stu-id="f1106-124">String</span></span>|<span data-ttu-id="f1106-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="f1106-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="f1106-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1106-126">servicePrincipalName</span></span>|<span data-ttu-id="f1106-127">String</span><span class="sxs-lookup"><span data-stu-id="f1106-127">String</span></span>|<span data-ttu-id="f1106-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="f1106-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="f1106-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f1106-129">ipAddress</span></span>|<span data-ttu-id="f1106-130">String</span><span class="sxs-lookup"><span data-stu-id="f1106-130">String</span></span>|<span data-ttu-id="f1106-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="f1106-131">IPAddress.</span></span>|
|<span data-ttu-id="f1106-132">userId</span><span class="sxs-lookup"><span data-stu-id="f1106-132">userId</span></span>|<span data-ttu-id="f1106-133">String</span><span class="sxs-lookup"><span data-stu-id="f1106-133">String</span></span>|<span data-ttu-id="f1106-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1106-134">User Id.</span></span>|
|<span data-ttu-id="f1106-135">усерролескопетагс</span><span class="sxs-lookup"><span data-stu-id="f1106-135">userRoleScopeTags</span></span>|<span data-ttu-id="f1106-136">Коллекция [ролескопетагинфо](../resources/intune-auditing-rolescopetaginfo.md)</span><span class="sxs-lookup"><span data-stu-id="f1106-136">[roleScopeTagInfo](../resources/intune-auditing-rolescopetaginfo.md) collection</span></span>|<span data-ttu-id="f1106-137">Список тегов области пользователя при выполнении аудита.</span><span class="sxs-lookup"><span data-stu-id="f1106-137">List of user scope tags when the audit was performed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1106-138">Связи</span><span class="sxs-lookup"><span data-stu-id="f1106-138">Relationships</span></span>
<span data-ttu-id="f1106-139">Нет</span><span class="sxs-lookup"><span data-stu-id="f1106-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1106-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1106-140">JSON Representation</span></span>
<span data-ttu-id="f1106-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1106-141">Here is a JSON representation of the resource.</span></span>
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



