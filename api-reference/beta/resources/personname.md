---
title: Тип ресурса personName
description: Тип ресурса personName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6212721774b9b7bc47a4e312d438f1b001a90bef
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521906"
---
# <a name="personname-resource-type"></a><span data-ttu-id="203e6-103">Тип ресурса personName</span><span class="sxs-lookup"><span data-stu-id="203e6-103">personName resource type</span></span>

<span data-ttu-id="203e6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="203e6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="203e6-105">Представляет сведения о расширенных именах, предоставленных пользователем или связанными с их учетной записью.</span><span class="sxs-lookup"><span data-stu-id="203e6-105">Represents extended name information provided by the user or which they have associated with their account.</span></span>

<span data-ttu-id="203e6-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="203e6-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="203e6-107">Методы</span><span class="sxs-lookup"><span data-stu-id="203e6-107">Methods</span></span>

| <span data-ttu-id="203e6-108">Метод</span><span class="sxs-lookup"><span data-stu-id="203e6-108">Method</span></span>                                     | <span data-ttu-id="203e6-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="203e6-109">Return Type</span></span>                 | <span data-ttu-id="203e6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="203e6-110">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="203e6-111">Получение personName</span><span class="sxs-lookup"><span data-stu-id="203e6-111">Get personName</span></span>](../api/personname-get.md) | [<span data-ttu-id="203e6-112">personName</span><span class="sxs-lookup"><span data-stu-id="203e6-112">personName</span></span>](personname.md) | <span data-ttu-id="203e6-113">Чтение свойств и связей объекта personName.</span><span class="sxs-lookup"><span data-stu-id="203e6-113">Read properties and relationships of personName object.</span></span> |
| <span data-ttu-id="203e6-114">[обновление](../api/personname-update.md).</span><span class="sxs-lookup"><span data-stu-id="203e6-114">[Update](../api/personname-update.md)</span></span>      | [<span data-ttu-id="203e6-115">personName</span><span class="sxs-lookup"><span data-stu-id="203e6-115">personName</span></span>](personname.md) | <span data-ttu-id="203e6-116">Обновление объекта personName.</span><span class="sxs-lookup"><span data-stu-id="203e6-116">Update personName object.</span></span>                               |
| <span data-ttu-id="203e6-117">[удаление](../api/personname-delete.md);</span><span class="sxs-lookup"><span data-stu-id="203e6-117">[Delete](../api/personname-delete.md)</span></span>      | <span data-ttu-id="203e6-118">Нет</span><span class="sxs-lookup"><span data-stu-id="203e6-118">None</span></span>                        | <span data-ttu-id="203e6-119">Удаление объекта personName.</span><span class="sxs-lookup"><span data-stu-id="203e6-119">Delete personName object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="203e6-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="203e6-120">Properties</span></span>

| <span data-ttu-id="203e6-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="203e6-121">Property</span></span>     | <span data-ttu-id="203e6-122">Тип</span><span class="sxs-lookup"><span data-stu-id="203e6-122">Type</span></span>                              | <span data-ttu-id="203e6-123">Описание</span><span class="sxs-lookup"><span data-stu-id="203e6-123">Description</span></span> |
|:-------------|:----------------------------------|:------------|
|<span data-ttu-id="203e6-124">displayName</span><span class="sxs-lookup"><span data-stu-id="203e6-124">displayName</span></span>   |<span data-ttu-id="203e6-125">Строка</span><span class="sxs-lookup"><span data-stu-id="203e6-125">String</span></span>                             | <span data-ttu-id="203e6-126">Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="203e6-126">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span> |
|<span data-ttu-id="203e6-127">первыми</span><span class="sxs-lookup"><span data-stu-id="203e6-127">first</span></span>         |<span data-ttu-id="203e6-128">String</span><span class="sxs-lookup"><span data-stu-id="203e6-128">String</span></span>                             | <span data-ttu-id="203e6-129">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="203e6-129">First Name of the user.</span></span>                                                                                      |
|<span data-ttu-id="203e6-130">initials</span><span class="sxs-lookup"><span data-stu-id="203e6-130">initials</span></span>      |<span data-ttu-id="203e6-131">String</span><span class="sxs-lookup"><span data-stu-id="203e6-131">String</span></span>                             | <span data-ttu-id="203e6-132">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="203e6-132">Initials of the user.</span></span>                                                                                        |
|<span data-ttu-id="203e6-133">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="203e6-133">languageTag</span></span>   |<span data-ttu-id="203e6-134">String</span><span class="sxs-lookup"><span data-stu-id="203e6-134">String</span></span>                             | <span data-ttu-id="203e6-135">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="203e6-135">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>                        |
|<span data-ttu-id="203e6-136">Фамили</span><span class="sxs-lookup"><span data-stu-id="203e6-136">last</span></span>          |<span data-ttu-id="203e6-137">String</span><span class="sxs-lookup"><span data-stu-id="203e6-137">String</span></span>                             | <span data-ttu-id="203e6-138">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="203e6-138">Last Name of the user.</span></span>                                                                                       |
|<span data-ttu-id="203e6-139">маиден</span><span class="sxs-lookup"><span data-stu-id="203e6-139">maiden</span></span>        |<span data-ttu-id="203e6-140">String</span><span class="sxs-lookup"><span data-stu-id="203e6-140">String</span></span>                             | <span data-ttu-id="203e6-141">Маиден имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="203e6-141">Maiden Name of the user.</span></span>                                                                                     |
|<span data-ttu-id="203e6-142">назван</span><span class="sxs-lookup"><span data-stu-id="203e6-142">middle</span></span>        |<span data-ttu-id="203e6-143">String</span><span class="sxs-lookup"><span data-stu-id="203e6-143">String</span></span>                             | <span data-ttu-id="203e6-144">Миддлие имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="203e6-144">Middlie Name of the user.</span></span>                                                                                    | 
|<span data-ttu-id="203e6-145">прозвищ</span><span class="sxs-lookup"><span data-stu-id="203e6-145">nickname</span></span>      |<span data-ttu-id="203e6-146">String</span><span class="sxs-lookup"><span data-stu-id="203e6-146">String</span></span>                             | <span data-ttu-id="203e6-147">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="203e6-147">Nickname of the user.</span></span>                                                                                        |
|<span data-ttu-id="203e6-148">произношение</span><span class="sxs-lookup"><span data-stu-id="203e6-148">pronunciation</span></span> |[<span data-ttu-id="203e6-149">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="203e6-149">yomiPersonName</span></span>](yomipersonname.md)| <span data-ttu-id="203e6-150">Руководство по произношению имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="203e6-150">Guidance on how to pronounce the users name.</span></span>                                                                 |
|<span data-ttu-id="203e6-151">суффикс</span><span class="sxs-lookup"><span data-stu-id="203e6-151">suffix</span></span>        |<span data-ttu-id="203e6-152">String</span><span class="sxs-lookup"><span data-stu-id="203e6-152">String</span></span>                             | <span data-ttu-id="203e6-153">Обозначения, используемые после имени пользователя (например, "доктор").</span><span class="sxs-lookup"><span data-stu-id="203e6-153">Designators used after the users name (eg: PhD.)</span></span>                                                             |
|<span data-ttu-id="203e6-154">title</span><span class="sxs-lookup"><span data-stu-id="203e6-154">title</span></span>         |<span data-ttu-id="203e6-155">String</span><span class="sxs-lookup"><span data-stu-id="203e6-155">String</span></span>                             | <span data-ttu-id="203e6-156">Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).</span><span class="sxs-lookup"><span data-stu-id="203e6-156">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="203e6-157">Связи</span><span class="sxs-lookup"><span data-stu-id="203e6-157">Relationships</span></span>

<span data-ttu-id="203e6-158">Нет</span><span class="sxs-lookup"><span data-stu-id="203e6-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="203e6-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="203e6-159">JSON representation</span></span>

<span data-ttu-id="203e6-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="203e6-160">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personName",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "initials": "String",
  "languageTag": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String",
  "nickname": "String",
  "pronunciation": {"@odata.type": "microsoft.graph.yomiPersonName"},
  "suffix": "String",
  "title": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->