---
title: Тип ресурса Жаурналлинес
description: Строка журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: cb9b20d7d88159dbddd2a18caa6db7fe52e5a601
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972917"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="d75da-103">Тип ресурса Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="d75da-103">journalLines resource type</span></span>
<span data-ttu-id="d75da-104">Представляет строку в журнале в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="d75da-104">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="d75da-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d75da-105">Methods</span></span>

| <span data-ttu-id="d75da-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d75da-106">Method</span></span>                                                    | <span data-ttu-id="d75da-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d75da-107">Return Type</span></span>|<span data-ttu-id="d75da-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d75da-108">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="d75da-109">Получение Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="d75da-109">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="d75da-110">Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="d75da-110">journalLines</span></span>|<span data-ttu-id="d75da-111">Получает строку журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-111">Gets a journal line.</span></span>   |
|[<span data-ttu-id="d75da-112">POST Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="d75da-112">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="d75da-113">Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="d75da-113">journalLines</span></span>|<span data-ttu-id="d75da-114">Создает строку журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-114">Creates a journal line.</span></span>|
|[<span data-ttu-id="d75da-115">Исправление Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="d75da-115">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="d75da-116">Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="d75da-116">journalLines</span></span>|<span data-ttu-id="d75da-117">Обновляет строку журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-117">Updates a journal line.</span></span>|
|[<span data-ttu-id="d75da-118">Удаление Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="d75da-118">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="d75da-119">none</span><span class="sxs-lookup"><span data-stu-id="d75da-119">none</span></span>        |<span data-ttu-id="d75da-120">Удаляет строку журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-120">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="d75da-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="d75da-121">Properties</span></span>
| <span data-ttu-id="d75da-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="d75da-122">Property</span></span>             | <span data-ttu-id="d75da-123">Тип</span><span class="sxs-lookup"><span data-stu-id="d75da-123">Type</span></span>                   |<span data-ttu-id="d75da-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d75da-124">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="d75da-125">id</span><span class="sxs-lookup"><span data-stu-id="d75da-125">id</span></span>                    |<span data-ttu-id="d75da-126">GUID</span><span class="sxs-lookup"><span data-stu-id="d75da-126">GUID</span></span>                    |<span data-ttu-id="d75da-127">Уникальный идентификатор строки журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-127">The unique ID of the journal line.</span></span> <span data-ttu-id="d75da-128">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="d75da-128">Non-editable.</span></span>                   |
|<span data-ttu-id="d75da-129">Жаурналдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="d75da-129">journalDisplayName</span></span>    |<span data-ttu-id="d75da-130">Строка, максимальный размер 10</span><span class="sxs-lookup"><span data-stu-id="d75da-130">string, maximum size 10</span></span> |<span data-ttu-id="d75da-131">Отображаемое имя журнала, к которому относится эта строка.</span><span class="sxs-lookup"><span data-stu-id="d75da-131">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="d75da-132">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d75da-132">Read-Only.</span></span>|
|<span data-ttu-id="d75da-133">lineNumber</span><span class="sxs-lookup"><span data-stu-id="d75da-133">lineNumber</span></span>            |<span data-ttu-id="d75da-134">целое</span><span class="sxs-lookup"><span data-stu-id="d75da-134">integer</span></span>                 |<span data-ttu-id="d75da-135">Номер строки журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-135">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="d75da-136">accountId</span><span class="sxs-lookup"><span data-stu-id="d75da-136">accountId</span></span>             |<span data-ttu-id="d75da-137">GUID</span><span class="sxs-lookup"><span data-stu-id="d75da-137">GUID</span></span>                    |<span data-ttu-id="d75da-138">Уникальный идентификатор учетной записи, с которой связана строка журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-138">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="d75da-139">Аккаунтнумбер</span><span class="sxs-lookup"><span data-stu-id="d75da-139">accountNumber</span></span>         |<span data-ttu-id="d75da-140">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="d75da-140">string, maximum size 20</span></span> |<span data-ttu-id="d75da-141">Номер учетной записи, с которой связана строка журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-141">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="d75da-142">Постингдате</span><span class="sxs-lookup"><span data-stu-id="d75da-142">postingDate</span></span>           |<span data-ttu-id="d75da-143">date</span><span class="sxs-lookup"><span data-stu-id="d75da-143">date</span></span>                    |<span data-ttu-id="d75da-144">Дата, когда строка журнала разносится.</span><span class="sxs-lookup"><span data-stu-id="d75da-144">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="d75da-145">Документнумбер</span><span class="sxs-lookup"><span data-stu-id="d75da-145">documentNumber</span></span>        |<span data-ttu-id="d75da-146">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="d75da-146">string, maximum size 20</span></span> |<span data-ttu-id="d75da-147">Указывает номер документа для строки журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-147">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="d75da-148">Екстерналдокументнумбер</span><span class="sxs-lookup"><span data-stu-id="d75da-148">externalDocumentNumber</span></span>|<span data-ttu-id="d75da-149">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="d75da-149">string, maximum size 20</span></span> |<span data-ttu-id="d75da-150">Указывает номер внешнего документа для строки журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-150">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="d75da-151">отступ</span><span class="sxs-lookup"><span data-stu-id="d75da-151">amount</span></span>                |<span data-ttu-id="d75da-152">числе</span><span class="sxs-lookup"><span data-stu-id="d75da-152">decimal</span></span>                 |<span data-ttu-id="d75da-153">Указывает общую сумму (включая НДС), из которой состоит строка журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-153">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="d75da-154">description</span><span class="sxs-lookup"><span data-stu-id="d75da-154">description</span></span>           |<span data-ttu-id="d75da-155">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="d75da-155">string, maximum size 50</span></span> |<span data-ttu-id="d75da-156">Описание строки журнала, предоставленное пользователем или созданным пользователем.</span><span class="sxs-lookup"><span data-stu-id="d75da-156">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="d75da-157">комментарий</span><span class="sxs-lookup"><span data-stu-id="d75da-157">comment</span></span>               |<span data-ttu-id="d75da-158">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="d75da-158">string, maximum size 250</span></span>|<span data-ttu-id="d75da-159">Заданный пользователем комментарий в строке журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-159">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="d75da-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d75da-160">lastModifiedDateTime</span></span>  |<span data-ttu-id="d75da-161">отличным</span><span class="sxs-lookup"><span data-stu-id="d75da-161">datetime</span></span>                |<span data-ttu-id="d75da-162">Дата и время последнего изменения строки журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-162">The last datetime the journal line was modified.</span></span> <span data-ttu-id="d75da-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d75da-163">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="d75da-164">Связи</span><span class="sxs-lookup"><span data-stu-id="d75da-164">Relationships</span></span>
<span data-ttu-id="d75da-165">Строка журнала является вложенной страницей журнала.</span><span class="sxs-lookup"><span data-stu-id="d75da-165">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="d75da-166">Прямой доступ к нему невозможен.</span><span class="sxs-lookup"><span data-stu-id="d75da-166">It cannot be accessed directly.</span></span>

<span data-ttu-id="d75da-167">Строка журнала может быть "родительским объектом" для строк измерения.</span><span class="sxs-lookup"><span data-stu-id="d75da-167">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="d75da-168">Учетная запись (accountId) должна существовать в таблице Accounts.</span><span class="sxs-lookup"><span data-stu-id="d75da-168">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d75da-169">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d75da-169">JSON representation</span></span>

<span data-ttu-id="d75da-170">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d75da-170">Here is a JSON representation of the resource.</span></span>


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
