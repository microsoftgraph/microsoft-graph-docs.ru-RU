---
title: тип ресурса tenantContactInformation
description: Представляет контакт в управляемом клиенте.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: b60005cf60a9ac1b96a3b650a853f8b198d27e48
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53403157"
---
# <a name="tenantcontactinformation-resource-type"></a><span data-ttu-id="d325a-103">тип ресурса tenantContactInformation</span><span class="sxs-lookup"><span data-stu-id="d325a-103">tenantContactInformation resource type</span></span>

<span data-ttu-id="d325a-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="d325a-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d325a-105">Представляет контакт в управляемом клиенте.</span><span class="sxs-lookup"><span data-stu-id="d325a-105">Represents a contact at a managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="d325a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d325a-106">Properties</span></span>
|<span data-ttu-id="d325a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d325a-107">Property</span></span>|<span data-ttu-id="d325a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d325a-108">Type</span></span>|<span data-ttu-id="d325a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d325a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d325a-110">email</span><span class="sxs-lookup"><span data-stu-id="d325a-110">email</span></span>|<span data-ttu-id="d325a-111">String</span><span class="sxs-lookup"><span data-stu-id="d325a-111">String</span></span>|<span data-ttu-id="d325a-112">Адрес электронной почты для контакта.</span><span class="sxs-lookup"><span data-stu-id="d325a-112">The email address for the contact.</span></span> <span data-ttu-id="d325a-113">Необязательный</span><span class="sxs-lookup"><span data-stu-id="d325a-113">Optional</span></span>|
|<span data-ttu-id="d325a-114">name</span><span class="sxs-lookup"><span data-stu-id="d325a-114">name</span></span>|<span data-ttu-id="d325a-115">String</span><span class="sxs-lookup"><span data-stu-id="d325a-115">String</span></span>|<span data-ttu-id="d325a-116">Имя контакта.</span><span class="sxs-lookup"><span data-stu-id="d325a-116">The name for the contact.</span></span> <span data-ttu-id="d325a-117">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d325a-117">Required.</span></span>|
|<span data-ttu-id="d325a-118">notes</span><span class="sxs-lookup"><span data-stu-id="d325a-118">notes</span></span>|<span data-ttu-id="d325a-119">String</span><span class="sxs-lookup"><span data-stu-id="d325a-119">String</span></span>|<span data-ttu-id="d325a-120">Заметки, связанные с контактом.</span><span class="sxs-lookup"><span data-stu-id="d325a-120">The notes associated with the contact.</span></span> <span data-ttu-id="d325a-121">Необязательный</span><span class="sxs-lookup"><span data-stu-id="d325a-121">Optional</span></span>|
|<span data-ttu-id="d325a-122">phone</span><span class="sxs-lookup"><span data-stu-id="d325a-122">phone</span></span>|<span data-ttu-id="d325a-123">String</span><span class="sxs-lookup"><span data-stu-id="d325a-123">String</span></span>|<span data-ttu-id="d325a-124">Номер телефона для контакта.</span><span class="sxs-lookup"><span data-stu-id="d325a-124">The phone number for the contact.</span></span> <span data-ttu-id="d325a-125">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="d325a-125">Optional.</span></span>|
|<span data-ttu-id="d325a-126">title</span><span class="sxs-lookup"><span data-stu-id="d325a-126">title</span></span>|<span data-ttu-id="d325a-127">String</span><span class="sxs-lookup"><span data-stu-id="d325a-127">String</span></span>|<span data-ttu-id="d325a-128">Название для контакта.</span><span class="sxs-lookup"><span data-stu-id="d325a-128">The title for the contact.</span></span> <span data-ttu-id="d325a-129">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d325a-129">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d325a-130">Связи</span><span class="sxs-lookup"><span data-stu-id="d325a-130">Relationships</span></span>
<span data-ttu-id="d325a-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d325a-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d325a-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d325a-132">JSON representation</span></span>
<span data-ttu-id="d325a-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d325a-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContactInformation",
  "name": "String",
  "title": "String",
  "email": "String",
  "phone": "String",
  "notes": "String"
}
```
