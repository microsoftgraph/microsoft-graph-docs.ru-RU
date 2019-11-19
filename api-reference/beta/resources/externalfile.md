---
title: Тип ресурса Екстерналфиле
description: Файл, индексируемый с помощью подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c3e51c27985927f5ea71f8ca618c4055a609fc06
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703751"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="453bb-103">Тип ресурса Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="453bb-103">externalFile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="453bb-104">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="453bb-104">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="453bb-105">Этот тип является производным от типа [екстерналитем](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="453bb-105">This type derives from the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="453bb-106">Методы</span><span class="sxs-lookup"><span data-stu-id="453bb-106">Methods</span></span>

| <span data-ttu-id="453bb-107">Метод</span><span class="sxs-lookup"><span data-stu-id="453bb-107">Method</span></span>                                                        | <span data-ttu-id="453bb-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="453bb-108">Return Type</span></span>  | <span data-ttu-id="453bb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="453bb-109">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="453bb-110">Создание Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="453bb-110">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="453bb-111">externalFile</span><span class="sxs-lookup"><span data-stu-id="453bb-111">externalFile</span></span> | <span data-ttu-id="453bb-112">Создайте объект Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="453bb-112">Create an externalFile.</span></span> |
| [<span data-ttu-id="453bb-113">Обновление Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="453bb-113">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="453bb-114">externalFile</span><span class="sxs-lookup"><span data-stu-id="453bb-114">externalFile</span></span> | <span data-ttu-id="453bb-115">Обновление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="453bb-115">Update an externalFile.</span></span> |
| [<span data-ttu-id="453bb-116">Удаление</span><span class="sxs-lookup"><span data-stu-id="453bb-116">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="453bb-117">Нет</span><span class="sxs-lookup"><span data-stu-id="453bb-117">None</span></span>         | <span data-ttu-id="453bb-118">Удаление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="453bb-118">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="453bb-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="453bb-119">Properties</span></span>

| <span data-ttu-id="453bb-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="453bb-120">Property</span></span>         | <span data-ttu-id="453bb-121">Тип</span><span class="sxs-lookup"><span data-stu-id="453bb-121">Type</span></span>                     | <span data-ttu-id="453bb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="453bb-122">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="453bb-123">списки</span><span class="sxs-lookup"><span data-stu-id="453bb-123">acl</span></span>              | <span data-ttu-id="453bb-124">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="453bb-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="453bb-125">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="453bb-125">An array of access control entries.</span></span> <span data-ttu-id="453bb-126">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="453bb-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="453bb-127">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="453bb-127">Required.</span></span> |
| <span data-ttu-id="453bb-128">content</span><span class="sxs-lookup"><span data-stu-id="453bb-128">content</span></span>          | <span data-ttu-id="453bb-129">String</span><span class="sxs-lookup"><span data-stu-id="453bb-129">String</span></span>                   | <span data-ttu-id="453bb-130">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="453bb-130">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="453bb-131">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="453bb-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="453bb-132">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="453bb-132">Optional.</span></span> |
| <span data-ttu-id="453bb-133">id</span><span class="sxs-lookup"><span data-stu-id="453bb-133">id</span></span>               | <span data-ttu-id="453bb-134">String</span><span class="sxs-lookup"><span data-stu-id="453bb-134">String</span></span>                   | <span data-ttu-id="453bb-135">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="453bb-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="453bb-136">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="453bb-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="453bb-137">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="453bb-137">Required.</span></span> |
| <span data-ttu-id="453bb-138">createdBy</span><span class="sxs-lookup"><span data-stu-id="453bb-138">createdBy</span></span>        | <span data-ttu-id="453bb-139">String</span><span class="sxs-lookup"><span data-stu-id="453bb-139">String</span></span>                   | <span data-ttu-id="453bb-140">Имя пользователя, создавшего файл.</span><span class="sxs-lookup"><span data-stu-id="453bb-140">The name of the user that created the file.</span></span> |
| <span data-ttu-id="453bb-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="453bb-141">createdDateTime</span></span>  | <span data-ttu-id="453bb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="453bb-142">DateTimeOffset</span></span>           | <span data-ttu-id="453bb-143">Дата и время создания файла.</span><span class="sxs-lookup"><span data-stu-id="453bb-143">The date and time that the file was created.</span></span> <span data-ttu-id="453bb-144">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="453bb-144">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="453bb-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="453bb-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="453bb-146">модулей</span><span class="sxs-lookup"><span data-stu-id="453bb-146">extension</span></span>        | <span data-ttu-id="453bb-147">String</span><span class="sxs-lookup"><span data-stu-id="453bb-147">String</span></span>                   | <span data-ttu-id="453bb-148">Расширение файла.</span><span class="sxs-lookup"><span data-stu-id="453bb-148">The file extension.</span></span>            |
| <span data-ttu-id="453bb-149">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="453bb-149">lastModifiedBy</span></span>   | <span data-ttu-id="453bb-150">String</span><span class="sxs-lookup"><span data-stu-id="453bb-150">String</span></span>                   | <span data-ttu-id="453bb-151">Имя пользователя, который последним изменил файл.</span><span class="sxs-lookup"><span data-stu-id="453bb-151">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="453bb-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="453bb-152">modifiedDateTime</span></span> | <span data-ttu-id="453bb-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="453bb-153">DateTimeOffset</span></span>           | <span data-ttu-id="453bb-154">Дата и время последнего изменения файла.</span><span class="sxs-lookup"><span data-stu-id="453bb-154">The date and time that the file was last modified.</span></span> <span data-ttu-id="453bb-155">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="453bb-155">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="453bb-156">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="453bb-156">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="453bb-157">name</span><span class="sxs-lookup"><span data-stu-id="453bb-157">name</span></span>             | <span data-ttu-id="453bb-158">Строка</span><span class="sxs-lookup"><span data-stu-id="453bb-158">String</span></span>                   | <span data-ttu-id="453bb-159">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="453bb-159">The file name.</span></span> <span data-ttu-id="453bb-160">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="453bb-160">Required.</span></span>       |
| <span data-ttu-id="453bb-161">size</span><span class="sxs-lookup"><span data-stu-id="453bb-161">size</span></span>             | <span data-ttu-id="453bb-162">Int64</span><span class="sxs-lookup"><span data-stu-id="453bb-162">Int64</span></span>                    | <span data-ttu-id="453bb-163">Размер файла в байтах.</span><span class="sxs-lookup"><span data-stu-id="453bb-163">The size of the file in bytes.</span></span> |
| <span data-ttu-id="453bb-164">title</span><span class="sxs-lookup"><span data-stu-id="453bb-164">title</span></span>            | <span data-ttu-id="453bb-165">String</span><span class="sxs-lookup"><span data-stu-id="453bb-165">String</span></span>                   | <span data-ttu-id="453bb-166">Заголовок файла.</span><span class="sxs-lookup"><span data-stu-id="453bb-166">The title of the file.</span></span>         |
| <span data-ttu-id="453bb-167">url</span><span class="sxs-lookup"><span data-stu-id="453bb-167">url</span></span>              | <span data-ttu-id="453bb-168">String</span><span class="sxs-lookup"><span data-stu-id="453bb-168">String</span></span>                   | <span data-ttu-id="453bb-169">URL-адрес для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="453bb-169">The URL to access the file.</span></span> <span data-ttu-id="453bb-170">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="453bb-170">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="453bb-171">Связи</span><span class="sxs-lookup"><span data-stu-id="453bb-171">Relationships</span></span>

<span data-ttu-id="453bb-172">Нет</span><span class="sxs-lookup"><span data-stu-id="453bb-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="453bb-173">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="453bb-173">JSON representation</span></span>

<span data-ttu-id="453bb-174">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="453bb-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalFile",
  "baseType": "microsoft.graph.externalItem"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": "String",
  "id": "String (identifier)",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "extension": "String",
  "lastModifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "name": "String",
  "size": 1024,
  "title": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
