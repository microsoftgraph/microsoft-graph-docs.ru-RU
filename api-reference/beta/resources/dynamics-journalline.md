---
title: Тип ресурса Жаурналлинес
description: Строка журнала в Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 8285a64b931ab18dac51cc20224877bbac74be90
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42503658"
---
# <a name="journallines-resource-type"></a><span data-ttu-id="54ec5-103">Тип ресурса Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="54ec5-103">journalLines resource type</span></span>

<span data-ttu-id="54ec5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="54ec5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54ec5-105">Представляет строку в журнале в Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="54ec5-105">Represents a line in a journal in Dynamics 365 Business Central.</span></span>

## <a name="methods"></a><span data-ttu-id="54ec5-106">Методы</span><span class="sxs-lookup"><span data-stu-id="54ec5-106">Methods</span></span>

| <span data-ttu-id="54ec5-107">Метод</span><span class="sxs-lookup"><span data-stu-id="54ec5-107">Method</span></span>                                                    | <span data-ttu-id="54ec5-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="54ec5-108">Return Type</span></span>|<span data-ttu-id="54ec5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="54ec5-109">Description</span></span>         |
|:----------------------------------------------------------|:-----------|:-------------------|
|[<span data-ttu-id="54ec5-110">Получение Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="54ec5-110">Get journalLines</span></span>](../api/dynamics-journalline-get.md)      |<span data-ttu-id="54ec5-111">жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="54ec5-111">journalLines</span></span>|<span data-ttu-id="54ec5-112">Получает строку журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-112">Gets a journal line.</span></span>   |
|[<span data-ttu-id="54ec5-113">POST Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="54ec5-113">Post journalLines</span></span>](../api/dynamics-create-journalline.md)  |<span data-ttu-id="54ec5-114">жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="54ec5-114">journalLines</span></span>|<span data-ttu-id="54ec5-115">Создает строку журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-115">Creates a journal line.</span></span>|
|[<span data-ttu-id="54ec5-116">Исправление Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="54ec5-116">Patch journalLines</span></span>](../api/dynamics-journalline-update.md) |<span data-ttu-id="54ec5-117">жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="54ec5-117">journalLines</span></span>|<span data-ttu-id="54ec5-118">Обновляет строку журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-118">Updates a journal line.</span></span>|
|[<span data-ttu-id="54ec5-119">Удаление Жаурналлинес</span><span class="sxs-lookup"><span data-stu-id="54ec5-119">Delete journalLines</span></span>](../api/dynamics-journalline-delete.md)|<span data-ttu-id="54ec5-120">нет</span><span class="sxs-lookup"><span data-stu-id="54ec5-120">none</span></span>        |<span data-ttu-id="54ec5-121">Удаляет строку журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-121">Deletes a journal line.</span></span>|

## <a name="properties"></a><span data-ttu-id="54ec5-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="54ec5-122">Properties</span></span>
| <span data-ttu-id="54ec5-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="54ec5-123">Property</span></span>             | <span data-ttu-id="54ec5-124">Тип</span><span class="sxs-lookup"><span data-stu-id="54ec5-124">Type</span></span>                   |<span data-ttu-id="54ec5-125">Описание</span><span class="sxs-lookup"><span data-stu-id="54ec5-125">Description</span></span>                                                        |
|:---------------------|:-----------------------|:------------------------------------------------------------------|
|<span data-ttu-id="54ec5-126">id</span><span class="sxs-lookup"><span data-stu-id="54ec5-126">id</span></span>                    |<span data-ttu-id="54ec5-127">GUID</span><span class="sxs-lookup"><span data-stu-id="54ec5-127">GUID</span></span>                    |<span data-ttu-id="54ec5-128">Уникальный идентификатор строки журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-128">The unique ID of the journal line.</span></span> <span data-ttu-id="54ec5-129">Не редактируемые.</span><span class="sxs-lookup"><span data-stu-id="54ec5-129">Non-editable.</span></span>                   |
|<span data-ttu-id="54ec5-130">жаурналдисплайнаме</span><span class="sxs-lookup"><span data-stu-id="54ec5-130">journalDisplayName</span></span>    |<span data-ttu-id="54ec5-131">Строка, максимальный размер 10</span><span class="sxs-lookup"><span data-stu-id="54ec5-131">string, maximum size 10</span></span> |<span data-ttu-id="54ec5-132">Отображаемое имя журнала, к которому относится эта строка.</span><span class="sxs-lookup"><span data-stu-id="54ec5-132">The display name of the journal that this line belongs to.</span></span> <span data-ttu-id="54ec5-133">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54ec5-133">Read-Only.</span></span>|
|<span data-ttu-id="54ec5-134">lineNumber</span><span class="sxs-lookup"><span data-stu-id="54ec5-134">lineNumber</span></span>            |<span data-ttu-id="54ec5-135">целое</span><span class="sxs-lookup"><span data-stu-id="54ec5-135">integer</span></span>                 |<span data-ttu-id="54ec5-136">Номер строки журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-136">The number of the journal line.</span></span>                                    |
|<span data-ttu-id="54ec5-137">accountId</span><span class="sxs-lookup"><span data-stu-id="54ec5-137">accountId</span></span>             |<span data-ttu-id="54ec5-138">GUID</span><span class="sxs-lookup"><span data-stu-id="54ec5-138">GUID</span></span>                    |<span data-ttu-id="54ec5-139">Уникальный идентификатор учетной записи, с которой связана строка журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-139">The unique ID of the account that the journal line is related to.</span></span>  |
|<span data-ttu-id="54ec5-140">аккаунтнумбер</span><span class="sxs-lookup"><span data-stu-id="54ec5-140">accountNumber</span></span>         |<span data-ttu-id="54ec5-141">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="54ec5-141">string, maximum size 20</span></span> |<span data-ttu-id="54ec5-142">Номер учетной записи, с которой связана строка журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-142">The number of the account that the journal line is related to.</span></span>     |
|<span data-ttu-id="54ec5-143">постингдате</span><span class="sxs-lookup"><span data-stu-id="54ec5-143">postingDate</span></span>           |<span data-ttu-id="54ec5-144">date</span><span class="sxs-lookup"><span data-stu-id="54ec5-144">date</span></span>                    |<span data-ttu-id="54ec5-145">Дата, когда строка журнала разносится.</span><span class="sxs-lookup"><span data-stu-id="54ec5-145">The date that the journal line is posted.</span></span>                          |
|<span data-ttu-id="54ec5-146">документнумбер</span><span class="sxs-lookup"><span data-stu-id="54ec5-146">documentNumber</span></span>        |<span data-ttu-id="54ec5-147">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="54ec5-147">string, maximum size 20</span></span> |<span data-ttu-id="54ec5-148">Указывает номер документа для строки журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-148">Specifies a document number for the journal line.</span></span>                  |
|<span data-ttu-id="54ec5-149">екстерналдокументнумбер</span><span class="sxs-lookup"><span data-stu-id="54ec5-149">externalDocumentNumber</span></span>|<span data-ttu-id="54ec5-150">Строка, максимальный размер 20</span><span class="sxs-lookup"><span data-stu-id="54ec5-150">string, maximum size 20</span></span> |<span data-ttu-id="54ec5-151">Указывает номер внешнего документа для строки журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-151">Specifies an external document number for the journal line.</span></span>        |
|<span data-ttu-id="54ec5-152">отступ</span><span class="sxs-lookup"><span data-stu-id="54ec5-152">amount</span></span>                |<span data-ttu-id="54ec5-153">числе</span><span class="sxs-lookup"><span data-stu-id="54ec5-153">decimal</span></span>                 |<span data-ttu-id="54ec5-154">Указывает общую сумму (включая НДС), из которой состоит строка журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-154">Specifies the total amount (including VAT) that the journal line consists of.</span></span>|
|<span data-ttu-id="54ec5-155">description</span><span class="sxs-lookup"><span data-stu-id="54ec5-155">description</span></span>           |<span data-ttu-id="54ec5-156">Строка, максимальный размер 50</span><span class="sxs-lookup"><span data-stu-id="54ec5-156">string, maximum size 50</span></span> |<span data-ttu-id="54ec5-157">Описание строки журнала, предоставленное пользователем или созданным пользователем.</span><span class="sxs-lookup"><span data-stu-id="54ec5-157">The description of the journal line, provided by the user or autocreated.</span></span>|
|<span data-ttu-id="54ec5-158">comment</span><span class="sxs-lookup"><span data-stu-id="54ec5-158">comment</span></span>               |<span data-ttu-id="54ec5-159">Строка, максимальный размер 250</span><span class="sxs-lookup"><span data-stu-id="54ec5-159">string, maximum size 250</span></span>|<span data-ttu-id="54ec5-160">Заданный пользователем комментарий в строке журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-160">A user specified comment on the journal line.</span></span>                      |
|<span data-ttu-id="54ec5-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="54ec5-161">lastModifiedDateTime</span></span>  |<span data-ttu-id="54ec5-162">datetime</span><span class="sxs-lookup"><span data-stu-id="54ec5-162">datetime</span></span>                |<span data-ttu-id="54ec5-163">Дата и время последнего изменения строки журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-163">The last datetime the journal line was modified.</span></span> <span data-ttu-id="54ec5-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="54ec5-164">Read-Only.</span></span>        |

## <a name="relationships"></a><span data-ttu-id="54ec5-165">Связи</span><span class="sxs-lookup"><span data-stu-id="54ec5-165">Relationships</span></span>
<span data-ttu-id="54ec5-166">Строка журнала является вложенной страницей журнала.</span><span class="sxs-lookup"><span data-stu-id="54ec5-166">A journal line is a subpage of a journal.</span></span> <span data-ttu-id="54ec5-167">Прямой доступ к нему невозможен.</span><span class="sxs-lookup"><span data-stu-id="54ec5-167">It cannot be accessed directly.</span></span>

<span data-ttu-id="54ec5-168">Строка журнала может быть "родительским объектом" для строк измерения.</span><span class="sxs-lookup"><span data-stu-id="54ec5-168">A journal line can be a "Parent Entity" of the dimension lines.</span></span>

<span data-ttu-id="54ec5-169">Учетная запись (accountId) должна существовать в таблице Accounts.</span><span class="sxs-lookup"><span data-stu-id="54ec5-169">An Account (accountId) must exist in the Accounts table.</span></span>


## <a name="json-representation"></a><span data-ttu-id="54ec5-170">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54ec5-170">JSON representation</span></span>

<span data-ttu-id="54ec5-171">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54ec5-171">Here is a JSON representation of the resource.</span></span>


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
