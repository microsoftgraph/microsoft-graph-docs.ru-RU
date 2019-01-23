---
title: Тип ресурса educationSynchronizationError
description: Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 397ac305fcacd789174c05ea36ab026826227475
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425815"
---
# <a name="educationsynchronizationerror-resource-type"></a><span data-ttu-id="c31d6-103">Тип ресурса educationSynchronizationError</span><span class="sxs-lookup"><span data-stu-id="c31d6-103">educationSynchronizationError resource type</span></span>

> <span data-ttu-id="c31d6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c31d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c31d6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c31d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c31d6-106">Представляет ошибку во время проверки данных профиля school и/или синхронизации. Уникальный ошибка создается для каждой записи, не удается проверить и/или синхронизация с Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="c31d6-106">Represents an error during school data profile validation and/or sync. A unique error is generated for every entry that fails to validate and/or synchronize with Azure Active Directory (Azure AD).</span></span>

## <a name="methods"></a><span data-ttu-id="c31d6-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c31d6-107">Methods</span></span>

| <span data-ttu-id="c31d6-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c31d6-108">Method</span></span> | <span data-ttu-id="c31d6-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c31d6-109">Return Type</span></span> | <span data-ttu-id="c31d6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c31d6-110">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="c31d6-111">Получение ошибки синхронизации</span><span class="sxs-lookup"><span data-stu-id="c31d6-111">Get synchronization errors</span></span>](../api/educationsynchronizationerrors-get.md) | <span data-ttu-id="c31d6-112">**educationSynchronizationError** коллекции</span><span class="sxs-lookup"><span data-stu-id="c31d6-112">**educationSynchronizationError** collection</span></span>| <span data-ttu-id="c31d6-113">Возвращает список ошибок синхронизации службы, связанные с профилем.</span><span class="sxs-lookup"><span data-stu-id="c31d6-113">Returns the list of synchronization errors associated with a profile.</span></span> |

## <a name="properties"></a><span data-ttu-id="c31d6-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="c31d6-114">Properties</span></span>

| <span data-ttu-id="c31d6-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="c31d6-115">Property</span></span> | <span data-ttu-id="c31d6-116">Тип</span><span class="sxs-lookup"><span data-stu-id="c31d6-116">Type</span></span> | <span data-ttu-id="c31d6-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c31d6-117">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c31d6-118">**entryType**</span><span class="sxs-lookup"><span data-stu-id="c31d6-118">**entryType**</span></span> | <span data-ttu-id="c31d6-119">string</span><span class="sxs-lookup"><span data-stu-id="c31d6-119">string</span></span> |  <span data-ttu-id="c31d6-120">Представляет сущности синхронизации (школа, раздел, учебы, преподаватель).</span><span class="sxs-lookup"><span data-stu-id="c31d6-120">Represents the sync entity (school, section, student, teacher).</span></span>       |
| <span data-ttu-id="c31d6-121">**errorCode**</span><span class="sxs-lookup"><span data-stu-id="c31d6-121">**errorCode**</span></span> | <span data-ttu-id="c31d6-122">string</span><span class="sxs-lookup"><span data-stu-id="c31d6-122">string</span></span> |  <span data-ttu-id="c31d6-123">Представляет код ошибки для этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="c31d6-123">Represents the error code for this error.</span></span>         |
| <span data-ttu-id="c31d6-124">**сообщение об ошибке**</span><span class="sxs-lookup"><span data-stu-id="c31d6-124">**errorMessage**</span></span> | <span data-ttu-id="c31d6-125">string</span><span class="sxs-lookup"><span data-stu-id="c31d6-125">string</span></span> |  <span data-ttu-id="c31d6-126">Содержит описание ошибки.</span><span class="sxs-lookup"><span data-stu-id="c31d6-126">Contains a description of the error.</span></span>        |
| <span data-ttu-id="c31d6-127">**joiningValue**</span><span class="sxs-lookup"><span data-stu-id="c31d6-127">**joiningValue**</span></span> | <span data-ttu-id="c31d6-128">string</span><span class="sxs-lookup"><span data-stu-id="c31d6-128">string</span></span> |  <span data-ttu-id="c31d6-129">Уникальный идентификатор для записи.</span><span class="sxs-lookup"><span data-stu-id="c31d6-129">The unique identifier for the entry.</span></span>         |
| <span data-ttu-id="c31d6-130">**recordedDateTime**</span><span class="sxs-lookup"><span data-stu-id="c31d6-130">**recordedDateTime**</span></span> | <span data-ttu-id="c31d6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c31d6-131">DateTimeOffset</span></span> | <span data-ttu-id="c31d6-132">Время возникновения этой ошибки.</span><span class="sxs-lookup"><span data-stu-id="c31d6-132">The time of occurrence of this error.</span></span>         |
| <span data-ttu-id="c31d6-133">**reportableIdentifier**</span><span class="sxs-lookup"><span data-stu-id="c31d6-133">**reportableIdentifier**</span></span> | <span data-ttu-id="c31d6-134">string</span><span class="sxs-lookup"><span data-stu-id="c31d6-134">string</span></span> | <span data-ttu-id="c31d6-135">Идентификатор элемента в этой записи об ошибках.</span><span class="sxs-lookup"><span data-stu-id="c31d6-135">The identifier of this error entry.</span></span>       |

## <a name="json-representation"></a><span data-ttu-id="c31d6-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c31d6-136">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
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
