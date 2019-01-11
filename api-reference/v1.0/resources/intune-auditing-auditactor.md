---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 14b4ce53d46897a84da8fab468ba2ad6aa99b30e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820050"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="f1c65-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="f1c65-103">auditActor resource type</span></span>

> <span data-ttu-id="f1c65-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1c65-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1c65-105">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="f1c65-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="f1c65-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f1c65-106">Properties</span></span>
|<span data-ttu-id="f1c65-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1c65-107">Property</span></span>|<span data-ttu-id="f1c65-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f1c65-108">Type</span></span>|<span data-ttu-id="f1c65-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f1c65-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1c65-110">type</span><span class="sxs-lookup"><span data-stu-id="f1c65-110">type</span></span>|<span data-ttu-id="f1c65-111">String</span><span class="sxs-lookup"><span data-stu-id="f1c65-111">String</span></span>|<span data-ttu-id="f1c65-112">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="f1c65-112">Actor Type.</span></span>|
|<span data-ttu-id="f1c65-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="f1c65-113">userPermissions</span></span>|<span data-ttu-id="f1c65-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="f1c65-114">String collection</span></span>|<span data-ttu-id="f1c65-115">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="f1c65-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="f1c65-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="f1c65-116">applicationId</span></span>|<span data-ttu-id="f1c65-117">String</span><span class="sxs-lookup"><span data-stu-id="f1c65-117">String</span></span>|<span data-ttu-id="f1c65-118">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="f1c65-118">AAD Application Id.</span></span>|
|<span data-ttu-id="f1c65-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="f1c65-119">applicationDisplayName</span></span>|<span data-ttu-id="f1c65-120">String</span><span class="sxs-lookup"><span data-stu-id="f1c65-120">String</span></span>|<span data-ttu-id="f1c65-121">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="f1c65-121">Name of the Application.</span></span>|
|<span data-ttu-id="f1c65-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1c65-122">userPrincipalName</span></span>|<span data-ttu-id="f1c65-123">String</span><span class="sxs-lookup"><span data-stu-id="f1c65-123">String</span></span>|<span data-ttu-id="f1c65-124">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="f1c65-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="f1c65-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="f1c65-125">servicePrincipalName</span></span>|<span data-ttu-id="f1c65-126">String</span><span class="sxs-lookup"><span data-stu-id="f1c65-126">String</span></span>|<span data-ttu-id="f1c65-127">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="f1c65-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="f1c65-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="f1c65-128">ipAddress</span></span>|<span data-ttu-id="f1c65-129">String</span><span class="sxs-lookup"><span data-stu-id="f1c65-129">String</span></span>|<span data-ttu-id="f1c65-130">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="f1c65-130">IPAddress.</span></span>|
|<span data-ttu-id="f1c65-131">userId</span><span class="sxs-lookup"><span data-stu-id="f1c65-131">userId</span></span>|<span data-ttu-id="f1c65-132">String</span><span class="sxs-lookup"><span data-stu-id="f1c65-132">String</span></span>|<span data-ttu-id="f1c65-133">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="f1c65-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1c65-134">Связи</span><span class="sxs-lookup"><span data-stu-id="f1c65-134">Relationships</span></span>
<span data-ttu-id="f1c65-135">Нет</span><span class="sxs-lookup"><span data-stu-id="f1c65-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f1c65-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f1c65-136">JSON Representation</span></span>
<span data-ttu-id="f1c65-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1c65-137">Here is a JSON representation of the resource.</span></span>
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



