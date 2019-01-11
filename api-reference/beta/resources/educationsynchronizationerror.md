---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: e5cf502c76aca816e75293ec8ac64cc544eeef7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852397"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="277b1-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="277b1-103">educationSynchronizationError resource type</span></span>

> <span data-ttu-id="277b1-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="277b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="277b1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="277b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="277b1-106">Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="277b1-106">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="277b1-107">Методы</span><span class="sxs-lookup"><span data-stu-id="277b1-107">Methods</span></span>

| <span data-ttu-id="277b1-108">Метод</span><span class="sxs-lookup"><span data-stu-id="277b1-108">Method</span></span> | <span data-ttu-id="277b1-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="277b1-109">Return Type</span></span> | <span data-ttu-id="277b1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="277b1-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="277b1-111">Получение ошибки синхронизации</span><span class="sxs-lookup"><span data-stu-id="277b1-111">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="277b1-112">**educationSynchronizationError** коллекции</span><span class="sxs-lookup"><span data-stu-id="277b1-112">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="277b1-113">Возвращает список ошибок синхронизации службы, связанные с профилем.</span><span class="sxs-lookup"><span data-stu-id="277b1-113">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="277b1-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="277b1-114">Properties</span></span>

| <span data-ttu-id="277b1-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="277b1-115">Property</span></span> | <span data-ttu-id="277b1-116">Тип</span><span class="sxs-lookup"><span data-stu-id="277b1-116">Type</span></span> | <span data-ttu-id="277b1-117">Описание</span><span class="sxs-lookup"><span data-stu-id="277b1-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="277b1-118">**entryType**</span><span class="sxs-lookup"><span data-stu-id="277b1-118">**entryType**</span></span> | <span data-ttu-id="277b1-119">string</span><span class="sxs-lookup"><span data-stu-id="277b1-119">string</span></span> |  <span data-ttu-id="277b1-120">Представляет сущности синхронизации (школа, раздел, учебы, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="277b1-120">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="277b1-121">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="277b1-121">**errorCode**</span></span> | <span data-ttu-id="277b1-122">string</span><span class="sxs-lookup"><span data-stu-id="277b1-122">string</span></span> |  <span data-ttu-id="277b1-123">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="277b1-123">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="277b1-124">**сообщение об ошибке**</span><span class="sxs-lookup"><span data-stu-id="277b1-124">**errorMessage**</span></span> | <span data-ttu-id="277b1-125">string</span><span class="sxs-lookup"><span data-stu-id="277b1-125">string</span></span> |  <span data-ttu-id="277b1-126">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="277b1-126">Contains a description of the error.</span></span>        |
| <span data-ttu-id="277b1-127">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="277b1-127">**joiningValue**</span></span> | <span data-ttu-id="277b1-128">string</span><span class="sxs-lookup"><span data-stu-id="277b1-128">string</span></span> |  <span data-ttu-id="277b1-129">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="277b1-129">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="277b1-130">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="277b1-130">**recordedDateTime**</span></span> | <span data-ttu-id="277b1-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="277b1-131">DateTimeOffset</span></span> | <span data-ttu-id="277b1-132">Время возникновения этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="277b1-132">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="277b1-133">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="277b1-133">**reportableIdentifier**</span></span> | <span data-ttu-id="277b1-134">string</span><span class="sxs-lookup"><span data-stu-id="277b1-134">string</span></span> | <span data-ttu-id="277b1-135">Идентификатор элемента в этой записи об ошибках.</span><span class="sxs-lookup"><span data-stu-id="277b1-135">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="277b1-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="277b1-136">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
