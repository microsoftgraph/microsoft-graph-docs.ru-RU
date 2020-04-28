---
title: Тип ресурса personName
description: Тип ресурса personName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e4927ba05443d4b54eaac3f54b7e0d3a8cd62159
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43227708"
---
# <a name="personname-resource-type"></a><span data-ttu-id="14247-103">Тип ресурса personName</span><span class="sxs-lookup"><span data-stu-id="14247-103">personName resource type</span></span>

<span data-ttu-id="14247-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14247-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14247-105">Представляет сведения о расширенных именах, предоставленных пользователем или связанными с их учетной записью.</span><span class="sxs-lookup"><span data-stu-id="14247-105">Represents extended name information provided by the user or which they have associated with their account.</span></span>

<span data-ttu-id="14247-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="14247-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="14247-107">Методы</span><span class="sxs-lookup"><span data-stu-id="14247-107">Methods</span></span>

| <span data-ttu-id="14247-108">Метод</span><span class="sxs-lookup"><span data-stu-id="14247-108">Method</span></span>                                     | <span data-ttu-id="14247-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="14247-109">Return Type</span></span>                 | <span data-ttu-id="14247-110">Описание</span><span class="sxs-lookup"><span data-stu-id="14247-110">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="14247-111">Получение personName</span><span class="sxs-lookup"><span data-stu-id="14247-111">Get personName</span></span>](../api/personname-get.md) | [<span data-ttu-id="14247-112">personName</span><span class="sxs-lookup"><span data-stu-id="14247-112">personName</span></span>](personname.md) | <span data-ttu-id="14247-113">Чтение свойств и связей объекта personName.</span><span class="sxs-lookup"><span data-stu-id="14247-113">Read properties and relationships of personName object.</span></span> |
| <span data-ttu-id="14247-114">[обновление](../api/personname-update.md).</span><span class="sxs-lookup"><span data-stu-id="14247-114">[Update](../api/personname-update.md)</span></span>      | [<span data-ttu-id="14247-115">personName</span><span class="sxs-lookup"><span data-stu-id="14247-115">personName</span></span>](personname.md) | <span data-ttu-id="14247-116">Обновление объекта personName.</span><span class="sxs-lookup"><span data-stu-id="14247-116">Update personName object.</span></span>                               |
| <span data-ttu-id="14247-117">[удаление](../api/personname-delete.md);</span><span class="sxs-lookup"><span data-stu-id="14247-117">[Delete](../api/personname-delete.md)</span></span>      | <span data-ttu-id="14247-118">Нет</span><span class="sxs-lookup"><span data-stu-id="14247-118">None</span></span>                        | <span data-ttu-id="14247-119">Удаление объекта personName.</span><span class="sxs-lookup"><span data-stu-id="14247-119">Delete personName object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="14247-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="14247-120">Properties</span></span>

| <span data-ttu-id="14247-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="14247-121">Property</span></span>     | <span data-ttu-id="14247-122">Тип</span><span class="sxs-lookup"><span data-stu-id="14247-122">Type</span></span>                              | <span data-ttu-id="14247-123">Описание</span><span class="sxs-lookup"><span data-stu-id="14247-123">Description</span></span>                                                                                                  |
|:-------------|:----------------------------------|:-------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="14247-124">displayName</span><span class="sxs-lookup"><span data-stu-id="14247-124">displayName</span></span>   |<span data-ttu-id="14247-125">Строка</span><span class="sxs-lookup"><span data-stu-id="14247-125">String</span></span>                             | <span data-ttu-id="14247-126">Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="14247-126">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span> |
|<span data-ttu-id="14247-127">первыми</span><span class="sxs-lookup"><span data-stu-id="14247-127">first</span></span>         |<span data-ttu-id="14247-128">String</span><span class="sxs-lookup"><span data-stu-id="14247-128">String</span></span>                             | <span data-ttu-id="14247-129">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="14247-129">First Name of the user.</span></span>                                                                                      |
|<span data-ttu-id="14247-130">initials</span><span class="sxs-lookup"><span data-stu-id="14247-130">initials</span></span>      |<span data-ttu-id="14247-131">String</span><span class="sxs-lookup"><span data-stu-id="14247-131">String</span></span>                             | <span data-ttu-id="14247-132">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="14247-132">Initials of the user.</span></span>                                                                                        |
|<span data-ttu-id="14247-133">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="14247-133">languageTag</span></span>   |<span data-ttu-id="14247-134">String</span><span class="sxs-lookup"><span data-stu-id="14247-134">String</span></span>                             | <span data-ttu-id="14247-135">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="14247-135">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>                        |
|<span data-ttu-id="14247-136">Фамили</span><span class="sxs-lookup"><span data-stu-id="14247-136">last</span></span>          |<span data-ttu-id="14247-137">String</span><span class="sxs-lookup"><span data-stu-id="14247-137">String</span></span>                             | <span data-ttu-id="14247-138">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="14247-138">Last Name of the user.</span></span>                                                                                       |
|<span data-ttu-id="14247-139">маиден</span><span class="sxs-lookup"><span data-stu-id="14247-139">maiden</span></span>        |<span data-ttu-id="14247-140">String</span><span class="sxs-lookup"><span data-stu-id="14247-140">String</span></span>                             | <span data-ttu-id="14247-141">Маиден имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="14247-141">Maiden Name of the user.</span></span>                                                                                     |
|<span data-ttu-id="14247-142">назван</span><span class="sxs-lookup"><span data-stu-id="14247-142">middle</span></span>        |<span data-ttu-id="14247-143">String</span><span class="sxs-lookup"><span data-stu-id="14247-143">String</span></span>                             | <span data-ttu-id="14247-144">Миддлие имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="14247-144">Middlie Name of the user.</span></span>                                                                                    |
|<span data-ttu-id="14247-145">прозвищ</span><span class="sxs-lookup"><span data-stu-id="14247-145">nickname</span></span>      |<span data-ttu-id="14247-146">String</span><span class="sxs-lookup"><span data-stu-id="14247-146">String</span></span>                             | <span data-ttu-id="14247-147">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="14247-147">Nickname of the user.</span></span>                                                                                        |
|<span data-ttu-id="14247-148">произношение</span><span class="sxs-lookup"><span data-stu-id="14247-148">pronunciation</span></span> |[<span data-ttu-id="14247-149">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="14247-149">yomiPersonName</span></span>](yomipersonname.md)| <span data-ttu-id="14247-150">Руководство по произношению имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="14247-150">Guidance on how to pronounce the users name.</span></span>                                                                 |
|<span data-ttu-id="14247-151">суффикс</span><span class="sxs-lookup"><span data-stu-id="14247-151">suffix</span></span>        |<span data-ttu-id="14247-152">String</span><span class="sxs-lookup"><span data-stu-id="14247-152">String</span></span>                             | <span data-ttu-id="14247-153">Обозначения, используемые после имени пользователя (например, "доктор").</span><span class="sxs-lookup"><span data-stu-id="14247-153">Designators used after the users name (eg: PhD.)</span></span>                                                             |
|<span data-ttu-id="14247-154">title</span><span class="sxs-lookup"><span data-stu-id="14247-154">title</span></span>         |<span data-ttu-id="14247-155">String</span><span class="sxs-lookup"><span data-stu-id="14247-155">String</span></span>                             | <span data-ttu-id="14247-156">Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).</span><span class="sxs-lookup"><span data-stu-id="14247-156">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="14247-157">Связи</span><span class="sxs-lookup"><span data-stu-id="14247-157">Relationships</span></span>

<span data-ttu-id="14247-158">Нет</span><span class="sxs-lookup"><span data-stu-id="14247-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="14247-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="14247-159">JSON representation</span></span>

<span data-ttu-id="14247-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="14247-160">The following is a JSON representation of the resource.</span></span>

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