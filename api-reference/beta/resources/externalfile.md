---
title: Тип ресурса Екстерналфиле
description: Файл, индексируемый с помощью подключения Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8a4f4e9bb9a782e71dd0c2f349baaacc5b61f480
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892600"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="03f4a-103">Тип ресурса Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="03f4a-103">externalFile resource type</span></span>

<span data-ttu-id="03f4a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03f4a-104">Namespace: microsoft.graph</span></span>

> [!CAUTION]
> <span data-ttu-id="03f4a-105">`externalFile` Тип устарел.</span><span class="sxs-lookup"><span data-stu-id="03f4a-105">The `externalFile` type has been deprecated.</span></span> <span data-ttu-id="03f4a-106">Разработчикам не следует использовать этот тип.</span><span class="sxs-lookup"><span data-stu-id="03f4a-106">Developers should not use this type.</span></span> <span data-ttu-id="03f4a-107">Внешние файлы по-прежнему могут индексироваться с помощью типа [екстерналитем](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="03f4a-107">External files may still be indexed using the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03f4a-108">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="03f4a-108">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="03f4a-109">Этот тип является производным от типа [екстерналитем](externalitem.md) .</span><span class="sxs-lookup"><span data-stu-id="03f4a-109">This type derives from the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="03f4a-110">Методы</span><span class="sxs-lookup"><span data-stu-id="03f4a-110">Methods</span></span>

| <span data-ttu-id="03f4a-111">Метод</span><span class="sxs-lookup"><span data-stu-id="03f4a-111">Method</span></span>                                                        | <span data-ttu-id="03f4a-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="03f4a-112">Return Type</span></span>  | <span data-ttu-id="03f4a-113">Описание</span><span class="sxs-lookup"><span data-stu-id="03f4a-113">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="03f4a-114">Создание Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="03f4a-114">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="03f4a-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="03f4a-115">externalFile</span></span> | <span data-ttu-id="03f4a-116">Создайте объект Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="03f4a-116">Create an externalFile.</span></span> |
| [<span data-ttu-id="03f4a-117">Обновление Екстерналфиле</span><span class="sxs-lookup"><span data-stu-id="03f4a-117">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="03f4a-118">externalFile</span><span class="sxs-lookup"><span data-stu-id="03f4a-118">externalFile</span></span> | <span data-ttu-id="03f4a-119">Обновление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="03f4a-119">Update an externalFile.</span></span> |
| <span data-ttu-id="03f4a-120">[удаление](../api/externalitem-delete.md);</span><span class="sxs-lookup"><span data-stu-id="03f4a-120">[Delete](../api/externalitem-delete.md)</span></span>                       | <span data-ttu-id="03f4a-121">Нет</span><span class="sxs-lookup"><span data-stu-id="03f4a-121">None</span></span>         | <span data-ttu-id="03f4a-122">Удаление Екстерналфиле.</span><span class="sxs-lookup"><span data-stu-id="03f4a-122">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="03f4a-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="03f4a-123">Properties</span></span>

| <span data-ttu-id="03f4a-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="03f4a-124">Property</span></span>         | <span data-ttu-id="03f4a-125">Тип</span><span class="sxs-lookup"><span data-stu-id="03f4a-125">Type</span></span>                     | <span data-ttu-id="03f4a-126">Описание</span><span class="sxs-lookup"><span data-stu-id="03f4a-126">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="03f4a-127">списки</span><span class="sxs-lookup"><span data-stu-id="03f4a-127">acl</span></span>              | <span data-ttu-id="03f4a-128">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="03f4a-128">[acl](acl.md) collection</span></span> | <span data-ttu-id="03f4a-129">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="03f4a-129">An array of access control entries.</span></span> <span data-ttu-id="03f4a-130">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="03f4a-130">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="03f4a-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03f4a-131">Required.</span></span> |
| <span data-ttu-id="03f4a-132">content</span><span class="sxs-lookup"><span data-stu-id="03f4a-132">content</span></span>          | <span data-ttu-id="03f4a-133">String</span><span class="sxs-lookup"><span data-stu-id="03f4a-133">String</span></span>                   | <span data-ttu-id="03f4a-134">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="03f4a-134">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="03f4a-135">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="03f4a-135">The text in this property is full-text indexed.</span></span> <span data-ttu-id="03f4a-136">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="03f4a-136">Optional.</span></span> |
| <span data-ttu-id="03f4a-137">id</span><span class="sxs-lookup"><span data-stu-id="03f4a-137">id</span></span>               | <span data-ttu-id="03f4a-138">String</span><span class="sxs-lookup"><span data-stu-id="03f4a-138">String</span></span>                   | <span data-ttu-id="03f4a-139">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="03f4a-139">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="03f4a-140">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="03f4a-140">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="03f4a-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03f4a-141">Required.</span></span> |
| <span data-ttu-id="03f4a-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="03f4a-142">createdBy</span></span>        | <span data-ttu-id="03f4a-143">String</span><span class="sxs-lookup"><span data-stu-id="03f4a-143">String</span></span>                   | <span data-ttu-id="03f4a-144">Имя пользователя, создавшего файл.</span><span class="sxs-lookup"><span data-stu-id="03f4a-144">The name of the user that created the file.</span></span> |
| <span data-ttu-id="03f4a-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03f4a-145">createdDateTime</span></span>  | <span data-ttu-id="03f4a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03f4a-146">DateTimeOffset</span></span>           | <span data-ttu-id="03f4a-147">Дата и время создания файла.</span><span class="sxs-lookup"><span data-stu-id="03f4a-147">The date and time that the file was created.</span></span> <span data-ttu-id="03f4a-148">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="03f4a-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03f4a-149">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="03f4a-149">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="03f4a-150">модулей</span><span class="sxs-lookup"><span data-stu-id="03f4a-150">extension</span></span>        | <span data-ttu-id="03f4a-151">String</span><span class="sxs-lookup"><span data-stu-id="03f4a-151">String</span></span>                   | <span data-ttu-id="03f4a-152">Расширение файла.</span><span class="sxs-lookup"><span data-stu-id="03f4a-152">The file extension.</span></span>            |
| <span data-ttu-id="03f4a-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="03f4a-153">lastModifiedBy</span></span>   | <span data-ttu-id="03f4a-154">String</span><span class="sxs-lookup"><span data-stu-id="03f4a-154">String</span></span>                   | <span data-ttu-id="03f4a-155">Имя пользователя, который последним изменил файл.</span><span class="sxs-lookup"><span data-stu-id="03f4a-155">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="03f4a-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03f4a-156">modifiedDateTime</span></span> | <span data-ttu-id="03f4a-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03f4a-157">DateTimeOffset</span></span>           | <span data-ttu-id="03f4a-158">Дата и время последнего изменения файла.</span><span class="sxs-lookup"><span data-stu-id="03f4a-158">The date and time that the file was last modified.</span></span> <span data-ttu-id="03f4a-159">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="03f4a-159">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="03f4a-160">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="03f4a-160">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span> |
| <span data-ttu-id="03f4a-161">name</span><span class="sxs-lookup"><span data-stu-id="03f4a-161">name</span></span>             | <span data-ttu-id="03f4a-162">Строка</span><span class="sxs-lookup"><span data-stu-id="03f4a-162">String</span></span>                   | <span data-ttu-id="03f4a-163">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="03f4a-163">The file name.</span></span> <span data-ttu-id="03f4a-164">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03f4a-164">Required.</span></span>       |
| <span data-ttu-id="03f4a-165">size</span><span class="sxs-lookup"><span data-stu-id="03f4a-165">size</span></span>             | <span data-ttu-id="03f4a-166">Int64</span><span class="sxs-lookup"><span data-stu-id="03f4a-166">Int64</span></span>                    | <span data-ttu-id="03f4a-167">Размер файла в байтах.</span><span class="sxs-lookup"><span data-stu-id="03f4a-167">The size of the file in bytes.</span></span> |
| <span data-ttu-id="03f4a-168">title</span><span class="sxs-lookup"><span data-stu-id="03f4a-168">title</span></span>            | <span data-ttu-id="03f4a-169">String</span><span class="sxs-lookup"><span data-stu-id="03f4a-169">String</span></span>                   | <span data-ttu-id="03f4a-170">Заголовок файла.</span><span class="sxs-lookup"><span data-stu-id="03f4a-170">The title of the file.</span></span>         |
| <span data-ttu-id="03f4a-171">url</span><span class="sxs-lookup"><span data-stu-id="03f4a-171">url</span></span>              | <span data-ttu-id="03f4a-172">String</span><span class="sxs-lookup"><span data-stu-id="03f4a-172">String</span></span>                   | <span data-ttu-id="03f4a-173">URL-адрес для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="03f4a-173">The URL to access the file.</span></span> <span data-ttu-id="03f4a-174">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03f4a-174">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="03f4a-175">Отношения</span><span class="sxs-lookup"><span data-stu-id="03f4a-175">Relationships</span></span>

<span data-ttu-id="03f4a-176">Нет</span><span class="sxs-lookup"><span data-stu-id="03f4a-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03f4a-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="03f4a-177">JSON representation</span></span>

<span data-ttu-id="03f4a-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="03f4a-178">The following is a JSON representation of the resource.</span></span>

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
