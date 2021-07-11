---
title: тип ресурса externalFile
description: Файл, индексацию с помощью Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 23a89cb83e85f16fc4cf2faa3c285bafb9fd66cf
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366550"
---
# <a name="externalfile-resource-type"></a><span data-ttu-id="95f18-103">тип ресурса externalFile</span><span class="sxs-lookup"><span data-stu-id="95f18-103">externalFile resource type</span></span>

<span data-ttu-id="95f18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95f18-104">Namespace: microsoft.graph</span></span>

> [!CAUTION]
> <span data-ttu-id="95f18-105">Тип `externalFile` был обесценим.</span><span class="sxs-lookup"><span data-stu-id="95f18-105">The `externalFile` type has been deprecated.</span></span> <span data-ttu-id="95f18-106">Разработчики не должны использовать этот тип.</span><span class="sxs-lookup"><span data-stu-id="95f18-106">Developers should not use this type.</span></span> <span data-ttu-id="95f18-107">Внешние файлы по-прежнему могут индексироваться с помощью [типа externalItem.](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="95f18-107">External files may still be indexed using the [externalItem](externalitem.md) type.</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="95f18-108">Элемент, индексация с помощью Поиск (Майкрософт) [подключения.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="95f18-108">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span> <span data-ttu-id="95f18-109">Этот тип происходит из [типа externalItem.](externalitem.md)</span><span class="sxs-lookup"><span data-stu-id="95f18-109">This type derives from the [externalItem](externalitem.md) type.</span></span>

## <a name="methods"></a><span data-ttu-id="95f18-110">Методы</span><span class="sxs-lookup"><span data-stu-id="95f18-110">Methods</span></span>

| <span data-ttu-id="95f18-111">Метод</span><span class="sxs-lookup"><span data-stu-id="95f18-111">Method</span></span>                                                        | <span data-ttu-id="95f18-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="95f18-112">Return Type</span></span>  | <span data-ttu-id="95f18-113">Описание</span><span class="sxs-lookup"><span data-stu-id="95f18-113">Description</span></span> |
|:--------------------------------------------------------------|:-------------|:--|
| [<span data-ttu-id="95f18-114">Создание externalFile</span><span class="sxs-lookup"><span data-stu-id="95f18-114">Create externalFile</span></span>](../api/externalconnection-put-items.md) | <span data-ttu-id="95f18-115">externalFile</span><span class="sxs-lookup"><span data-stu-id="95f18-115">externalFile</span></span> | <span data-ttu-id="95f18-116">Создайте externalFile.</span><span class="sxs-lookup"><span data-stu-id="95f18-116">Create an externalFile.</span></span> |
| [<span data-ttu-id="95f18-117">Обновление externalFile</span><span class="sxs-lookup"><span data-stu-id="95f18-117">Update externalFile</span></span>](../api/externalitem-update.md)          | <span data-ttu-id="95f18-118">externalFile</span><span class="sxs-lookup"><span data-stu-id="95f18-118">externalFile</span></span> | <span data-ttu-id="95f18-119">Обновление externalFile.</span><span class="sxs-lookup"><span data-stu-id="95f18-119">Update an externalFile.</span></span> |
| [<span data-ttu-id="95f18-120">Delete</span><span class="sxs-lookup"><span data-stu-id="95f18-120">Delete</span></span>](../api/externalitem-delete.md)                       | <span data-ttu-id="95f18-121">Нет</span><span class="sxs-lookup"><span data-stu-id="95f18-121">None</span></span>         | <span data-ttu-id="95f18-122">Удаление externalFile.</span><span class="sxs-lookup"><span data-stu-id="95f18-122">Delete an externalFile.</span></span> |

## <a name="properties"></a><span data-ttu-id="95f18-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="95f18-123">Properties</span></span>

| <span data-ttu-id="95f18-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="95f18-124">Property</span></span>         | <span data-ttu-id="95f18-125">Тип</span><span class="sxs-lookup"><span data-stu-id="95f18-125">Type</span></span>                     | <span data-ttu-id="95f18-126">Описание</span><span class="sxs-lookup"><span data-stu-id="95f18-126">Description</span></span>                    |
|:-----------------|:-------------------------|:-------------------------------|
| <span data-ttu-id="95f18-127">acl</span><span class="sxs-lookup"><span data-stu-id="95f18-127">acl</span></span>              | <span data-ttu-id="95f18-128">[коллекция acl](acl.md)</span><span class="sxs-lookup"><span data-stu-id="95f18-128">[acl](acl.md) collection</span></span> | <span data-ttu-id="95f18-129">Массив записей управления доступом.</span><span class="sxs-lookup"><span data-stu-id="95f18-129">An array of access control entries.</span></span> <span data-ttu-id="95f18-130">Каждая запись указывает доступ, предоставленный пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="95f18-130">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="95f18-131">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95f18-131">Required.</span></span> |
| <span data-ttu-id="95f18-132">content</span><span class="sxs-lookup"><span data-stu-id="95f18-132">content</span></span>          | <span data-ttu-id="95f18-133">String</span><span class="sxs-lookup"><span data-stu-id="95f18-133">String</span></span>                   | <span data-ttu-id="95f18-134">Простое текстовое представление содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="95f18-134">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="95f18-135">Текст в этом свойстве индексироваться с полным текстом.</span><span class="sxs-lookup"><span data-stu-id="95f18-135">The text in this property is full-text indexed.</span></span> <span data-ttu-id="95f18-136">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="95f18-136">Optional.</span></span> |
| <span data-ttu-id="95f18-137">id</span><span class="sxs-lookup"><span data-stu-id="95f18-137">id</span></span>               | <span data-ttu-id="95f18-138">String</span><span class="sxs-lookup"><span data-stu-id="95f18-138">String</span></span>                   | <span data-ttu-id="95f18-139">Уникальный ID элемента, предоставленного разработчиком, в пределах элемента, содержащего [externalConnection.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="95f18-139">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="95f18-140">Должно быть альфа-числом и не более 128 символов.</span><span class="sxs-lookup"><span data-stu-id="95f18-140">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="95f18-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95f18-141">Required.</span></span> |
| <span data-ttu-id="95f18-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="95f18-142">createdBy</span></span>        | <span data-ttu-id="95f18-143">String</span><span class="sxs-lookup"><span data-stu-id="95f18-143">String</span></span>                   | <span data-ttu-id="95f18-144">Имя пользователя, создав файл.</span><span class="sxs-lookup"><span data-stu-id="95f18-144">The name of the user that created the file.</span></span> |
| <span data-ttu-id="95f18-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95f18-145">createdDateTime</span></span>  | <span data-ttu-id="95f18-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95f18-146">DateTimeOffset</span></span>           | <span data-ttu-id="95f18-147">Дата и время создания файла.</span><span class="sxs-lookup"><span data-stu-id="95f18-147">The date and time that the file was created.</span></span> <span data-ttu-id="95f18-148">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="95f18-148">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="95f18-149">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="95f18-149">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
| <span data-ttu-id="95f18-150">расширение</span><span class="sxs-lookup"><span data-stu-id="95f18-150">extension</span></span>        | <span data-ttu-id="95f18-151">String</span><span class="sxs-lookup"><span data-stu-id="95f18-151">String</span></span>                   | <span data-ttu-id="95f18-152">Расширение файла.</span><span class="sxs-lookup"><span data-stu-id="95f18-152">The file extension.</span></span>            |
| <span data-ttu-id="95f18-153">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="95f18-153">lastModifiedBy</span></span>   | <span data-ttu-id="95f18-154">String</span><span class="sxs-lookup"><span data-stu-id="95f18-154">String</span></span>                   | <span data-ttu-id="95f18-155">Имя пользователя, который в последний раз изменил файл.</span><span class="sxs-lookup"><span data-stu-id="95f18-155">The name of the user that last modified the file.</span></span> |
| <span data-ttu-id="95f18-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95f18-156">modifiedDateTime</span></span> | <span data-ttu-id="95f18-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95f18-157">DateTimeOffset</span></span>           | <span data-ttu-id="95f18-158">Дата и время последнего изменения файла.</span><span class="sxs-lookup"><span data-stu-id="95f18-158">The date and time that the file was last modified.</span></span> <span data-ttu-id="95f18-159">Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="95f18-159">The DateTimeOffset type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="95f18-160">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="95f18-160">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span> |
| <span data-ttu-id="95f18-161">name</span><span class="sxs-lookup"><span data-stu-id="95f18-161">name</span></span>             | <span data-ttu-id="95f18-162">String</span><span class="sxs-lookup"><span data-stu-id="95f18-162">String</span></span>                   | <span data-ttu-id="95f18-163">Имя файла.</span><span class="sxs-lookup"><span data-stu-id="95f18-163">The file name.</span></span> <span data-ttu-id="95f18-164">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95f18-164">Required.</span></span>       |
| <span data-ttu-id="95f18-165">size</span><span class="sxs-lookup"><span data-stu-id="95f18-165">size</span></span>             | <span data-ttu-id="95f18-166">Int64</span><span class="sxs-lookup"><span data-stu-id="95f18-166">Int64</span></span>                    | <span data-ttu-id="95f18-167">Размер файла в bytes.</span><span class="sxs-lookup"><span data-stu-id="95f18-167">The size of the file in bytes.</span></span> |
| <span data-ttu-id="95f18-168">title</span><span class="sxs-lookup"><span data-stu-id="95f18-168">title</span></span>            | <span data-ttu-id="95f18-169">String</span><span class="sxs-lookup"><span data-stu-id="95f18-169">String</span></span>                   | <span data-ttu-id="95f18-170">Название файла.</span><span class="sxs-lookup"><span data-stu-id="95f18-170">The title of the file.</span></span>         |
| <span data-ttu-id="95f18-171">url</span><span class="sxs-lookup"><span data-stu-id="95f18-171">url</span></span>              | <span data-ttu-id="95f18-172">String</span><span class="sxs-lookup"><span data-stu-id="95f18-172">String</span></span>                   | <span data-ttu-id="95f18-173">URL-адрес для доступа к файлу.</span><span class="sxs-lookup"><span data-stu-id="95f18-173">The URL to access the file.</span></span> <span data-ttu-id="95f18-174">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="95f18-174">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="95f18-175">Связи</span><span class="sxs-lookup"><span data-stu-id="95f18-175">Relationships</span></span>

<span data-ttu-id="95f18-176">Нет</span><span class="sxs-lookup"><span data-stu-id="95f18-176">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95f18-177">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95f18-177">JSON representation</span></span>

<span data-ttu-id="95f18-178">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95f18-178">The following is a JSON representation of the resource.</span></span>

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


