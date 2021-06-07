---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ab8fc9f78fc647c82be80105cb3547e6a7a45f7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755580"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="8b260-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="8b260-103">auditActor resource type</span></span>

<span data-ttu-id="8b260-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b260-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b260-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8b260-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b260-106">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="8b260-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="8b260-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8b260-107">Properties</span></span>
|<span data-ttu-id="8b260-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8b260-108">Property</span></span>|<span data-ttu-id="8b260-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8b260-109">Type</span></span>|<span data-ttu-id="8b260-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8b260-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b260-111">type</span><span class="sxs-lookup"><span data-stu-id="8b260-111">type</span></span>|<span data-ttu-id="8b260-112">String</span><span class="sxs-lookup"><span data-stu-id="8b260-112">String</span></span>|<span data-ttu-id="8b260-113">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="8b260-113">Actor Type.</span></span>|
|<span data-ttu-id="8b260-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="8b260-114">userPermissions</span></span>|<span data-ttu-id="8b260-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8b260-115">String collection</span></span>|<span data-ttu-id="8b260-116">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="8b260-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="8b260-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="8b260-117">applicationId</span></span>|<span data-ttu-id="8b260-118">String</span><span class="sxs-lookup"><span data-stu-id="8b260-118">String</span></span>|<span data-ttu-id="8b260-119">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="8b260-119">AAD Application Id.</span></span>|
|<span data-ttu-id="8b260-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="8b260-120">applicationDisplayName</span></span>|<span data-ttu-id="8b260-121">String</span><span class="sxs-lookup"><span data-stu-id="8b260-121">String</span></span>|<span data-ttu-id="8b260-122">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="8b260-122">Name of the Application.</span></span>|
|<span data-ttu-id="8b260-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b260-123">userPrincipalName</span></span>|<span data-ttu-id="8b260-124">String</span><span class="sxs-lookup"><span data-stu-id="8b260-124">String</span></span>|<span data-ttu-id="8b260-125">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="8b260-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="8b260-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b260-126">servicePrincipalName</span></span>|<span data-ttu-id="8b260-127">String</span><span class="sxs-lookup"><span data-stu-id="8b260-127">String</span></span>|<span data-ttu-id="8b260-128">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="8b260-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="8b260-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="8b260-129">ipAddress</span></span>|<span data-ttu-id="8b260-130">String</span><span class="sxs-lookup"><span data-stu-id="8b260-130">String</span></span>|<span data-ttu-id="8b260-131">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="8b260-131">IPAddress.</span></span>|
|<span data-ttu-id="8b260-132">userId</span><span class="sxs-lookup"><span data-stu-id="8b260-132">userId</span></span>|<span data-ttu-id="8b260-133">String</span><span class="sxs-lookup"><span data-stu-id="8b260-133">String</span></span>|<span data-ttu-id="8b260-134">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b260-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b260-135">Связи</span><span class="sxs-lookup"><span data-stu-id="8b260-135">Relationships</span></span>
<span data-ttu-id="8b260-136">Нет</span><span class="sxs-lookup"><span data-stu-id="8b260-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b260-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8b260-137">JSON Representation</span></span>
<span data-ttu-id="8b260-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8b260-138">Here is a JSON representation of the resource.</span></span>
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




