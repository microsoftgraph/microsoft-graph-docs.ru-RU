---
title: Тип ресурса auditActor
description: Класс, содержащий свойства субъекта аудита.
author: tfitzmac
ms.openlocfilehash: de2fc78bcc02565da102beb57c077646effc443b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325020"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="a20ab-103">Тип ресурса auditActor</span><span class="sxs-lookup"><span data-stu-id="a20ab-103">auditActor resource type</span></span>

> <span data-ttu-id="a20ab-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a20ab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a20ab-105">Класс, содержащий свойства субъекта аудита.</span><span class="sxs-lookup"><span data-stu-id="a20ab-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="a20ab-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a20ab-106">Properties</span></span>
|<span data-ttu-id="a20ab-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a20ab-107">Property</span></span>|<span data-ttu-id="a20ab-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a20ab-108">Type</span></span>|<span data-ttu-id="a20ab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a20ab-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a20ab-110">type</span><span class="sxs-lookup"><span data-stu-id="a20ab-110">type</span></span>|<span data-ttu-id="a20ab-111">String</span><span class="sxs-lookup"><span data-stu-id="a20ab-111">String</span></span>|<span data-ttu-id="a20ab-112">Тип субъекта.</span><span class="sxs-lookup"><span data-stu-id="a20ab-112">Actor Type.</span></span>|
|<span data-ttu-id="a20ab-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="a20ab-113">userPermissions</span></span>|<span data-ttu-id="a20ab-114">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="a20ab-114">String collection</span></span>|<span data-ttu-id="a20ab-115">Список разрешений пользователей во время аудита.</span><span class="sxs-lookup"><span data-stu-id="a20ab-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="a20ab-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="a20ab-116">applicationId</span></span>|<span data-ttu-id="a20ab-117">String</span><span class="sxs-lookup"><span data-stu-id="a20ab-117">String</span></span>|<span data-ttu-id="a20ab-118">ИД приложения AAD.</span><span class="sxs-lookup"><span data-stu-id="a20ab-118">AAD Application Id.</span></span>|
|<span data-ttu-id="a20ab-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="a20ab-119">applicationDisplayName</span></span>|<span data-ttu-id="a20ab-120">String</span><span class="sxs-lookup"><span data-stu-id="a20ab-120">String</span></span>|<span data-ttu-id="a20ab-121">Имя приложения.</span><span class="sxs-lookup"><span data-stu-id="a20ab-121">Name of the Application.</span></span>|
|<span data-ttu-id="a20ab-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a20ab-122">userPrincipalName</span></span>|<span data-ttu-id="a20ab-123">String</span><span class="sxs-lookup"><span data-stu-id="a20ab-123">String</span></span>|<span data-ttu-id="a20ab-124">Имя участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="a20ab-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="a20ab-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="a20ab-125">servicePrincipalName</span></span>|<span data-ttu-id="a20ab-126">String</span><span class="sxs-lookup"><span data-stu-id="a20ab-126">String</span></span>|<span data-ttu-id="a20ab-127">Имя субъекта-службы (SPN).</span><span class="sxs-lookup"><span data-stu-id="a20ab-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="a20ab-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="a20ab-128">ipAddress</span></span>|<span data-ttu-id="a20ab-129">String</span><span class="sxs-lookup"><span data-stu-id="a20ab-129">String</span></span>|<span data-ttu-id="a20ab-130">IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="a20ab-130">IPAddress.</span></span>|
|<span data-ttu-id="a20ab-131">userId</span><span class="sxs-lookup"><span data-stu-id="a20ab-131">userId</span></span>|<span data-ttu-id="a20ab-132">String</span><span class="sxs-lookup"><span data-stu-id="a20ab-132">String</span></span>|<span data-ttu-id="a20ab-133">ИД пользователя.</span><span class="sxs-lookup"><span data-stu-id="a20ab-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a20ab-134">Связи</span><span class="sxs-lookup"><span data-stu-id="a20ab-134">Relationships</span></span>
<span data-ttu-id="a20ab-135">Нет</span><span class="sxs-lookup"><span data-stu-id="a20ab-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a20ab-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a20ab-136">JSON Representation</span></span>
<span data-ttu-id="a20ab-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a20ab-137">Here is a JSON representation of the resource.</span></span>
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



