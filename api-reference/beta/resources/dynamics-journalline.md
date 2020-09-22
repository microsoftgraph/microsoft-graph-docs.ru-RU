---
title: Тип ресурса Жаурналлинес
description: Строка журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 99d06b5a49bd2881ea6f329e8b0d3692a25444b4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013799"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="f85df-103">Тип ресурса Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="f85df-103">journalLines resource type</span></span>

<span data-ttu-id="f85df-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f85df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f85df-105">Представляет строку в журнале в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="f85df-105">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="f85df-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f85df-106">Methods</span></span>

| <span data-ttu-id="f85df-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f85df-107">Method</span></span>                                                    | <span data-ttu-id="f85df-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f85df-108">Return Type</span></span>|<span data-ttu-id="f85df-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f85df-109">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="f85df-110">Получение Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="f85df-110">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="f85df-111">жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="f85df-111">journalLines</span></span>|<span data-ttu-id="f85df-112">Получает строку журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-112">Gets a journal line.</span></span>   |
|[<span data-ttu-id="f85df-113">POST Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="f85df-113">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="f85df-114">жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="f85df-114">journalLines</span></span>|<span data-ttu-id="f85df-115">Создает строку журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-115">Creates a journal line.</span></span>|
|[<span data-ttu-id="f85df-116">Исправление Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="f85df-116">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="f85df-117">жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="f85df-117">journalLines</span></span>|<span data-ttu-id="f85df-118">Обновляет строку журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-118">Updates a journal line.</span></span>|
|[<span data-ttu-id="f85df-119">Удаление Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="f85df-119">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="f85df-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f85df-120">none</span></span>        |<span data-ttu-id="f85df-121">Удаляет строку журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-121">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="f85df-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="f85df-122">Properties</span></span>
| <span data-ttu-id="f85df-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="f85df-123">Property</span></span>             | <span data-ttu-id="f85df-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f85df-124">Type</span></span>                   |<span data-ttu-id="f85df-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f85df-125">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="f85df-126">id</span><span class="sxs-lookup"><span data-stu-id="f85df-126">id</span></span>                    |<span data-ttu-id="f85df-127">GUID</span><span class="sxs-lookup"><span data-stu-id="f85df-127">GUID</span></span>                    |<span data-ttu-id="f85df-128">Уникальный идентификатор строки журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-128">The unique ID of the journal line.</span></span> <span data-ttu-id="f85df-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="f85df-129">Non-editable.</span></span>                   |
|<span data-ttu-id="f85df-130">жаурналдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="f85df-130">journalDisplayName</span></span>    |<span data-ttu-id="f85df-131">Строка, максимальный размер 10</span><span class="sxs-lookup"><span data-stu-id="f85df-131">string, maximum size 10</span></span> |<span data-ttu-id="f85df-132">Отображаемое имя журнала, к которому относится эта строка.</span><span class="sxs-lookup"><span data-stu-id="f85df-132">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="f85df-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f85df-133">Read-Only.</span></span>|
|<span data-ttu-id="f85df-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="f85df-134">lineNumber</span></span>            |<span data-ttu-id="f85df-135">целое</span><span class="sxs-lookup"><span data-stu-id="f85df-135">integer</span></span>                 |<span data-ttu-id="f85df-136">Номер строки журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-136">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="f85df-137">accountId</span><span class="sxs-lookup"><span data-stu-id="f85df-137">accountId</span></span>             |<span data-ttu-id="f85df-138">GUID</span><span class="sxs-lookup"><span data-stu-id="f85df-138">GUID</span></span>                    |<span data-ttu-id="f85df-139">Уникальный идентификатор учетной записи, с которой связана строка журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-139">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="f85df-140">аккаунтнумбер</span><span class="sxs-lookup"><span data-stu-id="f85df-140">accountNumber</span></span>         |<span data-ttu-id="f85df-141">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="f85df-141">string, maximum size 20</span></span> |<span data-ttu-id="f85df-142">Номер учетной записи, с которой связана строка журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-142">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="f85df-143">постингдате</span><span class="sxs-lookup"><span data-stu-id="f85df-143">postingDate</span></span>           |<span data-ttu-id="f85df-144">date</span><span class="sxs-lookup"><span data-stu-id="f85df-144">date</span></span>                    |<span data-ttu-id="f85df-145">Дата, когда строка журнала разносится.</span><span class="sxs-lookup"><span data-stu-id="f85df-145">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="f85df-146">документнумбер</span><span class="sxs-lookup"><span data-stu-id="f85df-146">documentNumber</span></span>        |<span data-ttu-id="f85df-147">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="f85df-147">string, maximum size 20</span></span> |<span data-ttu-id="f85df-148">Указывает номер документа для строки журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-148">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="f85df-149">екстерналдокументнумбер</span><span class="sxs-lookup"><span data-stu-id="f85df-149">externalDocumentNumber</span></span>|<span data-ttu-id="f85df-150">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="f85df-150">string, maximum size 20</span></span> |<span data-ttu-id="f85df-151">Указывает номер внешнего документа для строки журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-151">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="f85df-152">отступ</span><span class="sxs-lookup"><span data-stu-id="f85df-152">amount</span></span>                |<span data-ttu-id="f85df-153">числе</span><span class="sxs-lookup"><span data-stu-id="f85df-153">decimal</span></span>                 |<span data-ttu-id="f85df-154">Указывает общую сумму (включая НДС), из которой состоит строка журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-154">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="f85df-155">description</span><span class="sxs-lookup"><span data-stu-id="f85df-155">description</span></span>           |<span data-ttu-id="f85df-156">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="f85df-156">string, maximum size 50</span></span> |<span data-ttu-id="f85df-157">Описание строки журнала, предоставленное пользователем или созданным пользователем.</span><span class="sxs-lookup"><span data-stu-id="f85df-157">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="f85df-158">comment</span><span class="sxs-lookup"><span data-stu-id="f85df-158">comment</span></span>               |<span data-ttu-id="f85df-159">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="f85df-159">string, maximum size 250</span></span>|<span data-ttu-id="f85df-160">Заданный пользователем комментарий в строке журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-160">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="f85df-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f85df-161">lastModifiedDateTime</span></span>  |<span data-ttu-id="f85df-162">datetime</span><span class="sxs-lookup"><span data-stu-id="f85df-162">datetime</span></span>                |<span data-ttu-id="f85df-163">Дата и время последнего изменения строки журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-163">The last datetime the journal line was modified.</span></span> <span data-ttu-id="f85df-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f85df-164">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="f85df-165">Связи</span><span class="sxs-lookup"><span data-stu-id="f85df-165">Relationships</span></span>
<span data-ttu-id="f85df-166">Строка журнала является вложенной страницей журнала.</span><span class="sxs-lookup"><span data-stu-id="f85df-166">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="f85df-167">Прямой доступ к нему невозможен.</span><span class="sxs-lookup"><span data-stu-id="f85df-167">It cannot be accessed directly.</span></span>

<span data-ttu-id="f85df-168">Строка журнала может быть "родительским объектом" для строк измерения.</span><span class="sxs-lookup"><span data-stu-id="f85df-168">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="f85df-169">Учетная запись (accountId) должна существовать в таблице Accounts.</span><span class="sxs-lookup"><span data-stu-id="f85df-169">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f85df-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f85df-170">JSON representation</span></span>

<span data-ttu-id="f85df-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f85df-171">Here is a JSON representation of the resource.</span></span>


```json
{
    "id": "GUID",
    "journalDisplayName": "string",
    "lineNumber": "integer",
    "accountId": "GUID",
    "accountNumber": "string",
    "postingDate": "date",
    "documentNumber": "string",
    "externalDocumentNumber": "string",
    "amount": "decimal",
    "description": "string",
    "comment": "string",
    "lastModifiedDateTime": "datetime"
}
```


