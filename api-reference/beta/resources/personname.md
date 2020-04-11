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
# <a name="personname-resource-type"></a><span data-ttu-id="611e8-103">Тип ресурса personName</span><span class="sxs-lookup"><span data-stu-id="611e8-103">personName resource type</span></span>

<span data-ttu-id="611e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="611e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="611e8-105">Представляет сведения о расширенных именах, предоставленных пользователем или связанными с их учетной записью.</span><span class="sxs-lookup"><span data-stu-id="611e8-105">Represents extended name information provided by the user or which they have associated with their account.</span></span>

<span data-ttu-id="611e8-106">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="611e8-106">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="611e8-107">Методы</span><span class="sxs-lookup"><span data-stu-id="611e8-107">Methods</span></span>

| <span data-ttu-id="611e8-108">Метод</span><span class="sxs-lookup"><span data-stu-id="611e8-108">Method</span></span>                                     | <span data-ttu-id="611e8-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="611e8-109">Return Type</span></span>                 | <span data-ttu-id="611e8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="611e8-110">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="611e8-111">Получение personName</span><span class="sxs-lookup"><span data-stu-id="611e8-111">Get personName</span></span>](../api/personname-get.md) | [<span data-ttu-id="611e8-112">personName</span><span class="sxs-lookup"><span data-stu-id="611e8-112">personName</span></span>](personname.md) | <span data-ttu-id="611e8-113">Чтение свойств и связей объекта personName.</span><span class="sxs-lookup"><span data-stu-id="611e8-113">Read properties and relationships of personName object.</span></span> |
| [<span data-ttu-id="611e8-114">Обновление</span><span class="sxs-lookup"><span data-stu-id="611e8-114">Update</span></span>](../api/personname-update.md)      | [<span data-ttu-id="611e8-115">personName</span><span class="sxs-lookup"><span data-stu-id="611e8-115">personName</span></span>](personname.md) | <span data-ttu-id="611e8-116">Обновление объекта personName.</span><span class="sxs-lookup"><span data-stu-id="611e8-116">Update personName object.</span></span>                               |
| [<span data-ttu-id="611e8-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="611e8-117">Delete</span></span>](../api/personname-delete.md)      | <span data-ttu-id="611e8-118">Нет</span><span class="sxs-lookup"><span data-stu-id="611e8-118">None</span></span>                        | <span data-ttu-id="611e8-119">Удаление объекта personName.</span><span class="sxs-lookup"><span data-stu-id="611e8-119">Delete personName object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="611e8-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="611e8-120">Properties</span></span>

| <span data-ttu-id="611e8-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="611e8-121">Property</span></span>     | <span data-ttu-id="611e8-122">Тип</span><span class="sxs-lookup"><span data-stu-id="611e8-122">Type</span></span>                              | <span data-ttu-id="611e8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="611e8-123">Description</span></span>                                                                                                  |
|:-------------|:----------------------------------|:-------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="611e8-124">displayName</span><span class="sxs-lookup"><span data-stu-id="611e8-124">displayName</span></span>   |<span data-ttu-id="611e8-125">Строка</span><span class="sxs-lookup"><span data-stu-id="611e8-125">String</span></span>                             | <span data-ttu-id="611e8-126">Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="611e8-126">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span> |
|<span data-ttu-id="611e8-127">первыми</span><span class="sxs-lookup"><span data-stu-id="611e8-127">first</span></span>         |<span data-ttu-id="611e8-128">String</span><span class="sxs-lookup"><span data-stu-id="611e8-128">String</span></span>                             | <span data-ttu-id="611e8-129">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="611e8-129">First Name of the user.</span></span>                                                                                      |
|<span data-ttu-id="611e8-130">initials</span><span class="sxs-lookup"><span data-stu-id="611e8-130">initials</span></span>      |<span data-ttu-id="611e8-131">String</span><span class="sxs-lookup"><span data-stu-id="611e8-131">String</span></span>                             | <span data-ttu-id="611e8-132">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="611e8-132">Initials of the user.</span></span>                                                                                        |
|<span data-ttu-id="611e8-133">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="611e8-133">languageTag</span></span>   |<span data-ttu-id="611e8-134">String</span><span class="sxs-lookup"><span data-stu-id="611e8-134">String</span></span>                             | <span data-ttu-id="611e8-135">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="611e8-135">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>                        |
|<span data-ttu-id="611e8-136">Фамили</span><span class="sxs-lookup"><span data-stu-id="611e8-136">last</span></span>          |<span data-ttu-id="611e8-137">String</span><span class="sxs-lookup"><span data-stu-id="611e8-137">String</span></span>                             | <span data-ttu-id="611e8-138">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="611e8-138">Last Name of the user.</span></span>                                                                                       |
|<span data-ttu-id="611e8-139">маиден</span><span class="sxs-lookup"><span data-stu-id="611e8-139">maiden</span></span>        |<span data-ttu-id="611e8-140">String</span><span class="sxs-lookup"><span data-stu-id="611e8-140">String</span></span>                             | <span data-ttu-id="611e8-141">Маиден имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="611e8-141">Maiden Name of the user.</span></span>                                                                                     |
|<span data-ttu-id="611e8-142">назван</span><span class="sxs-lookup"><span data-stu-id="611e8-142">middle</span></span>        |<span data-ttu-id="611e8-143">String</span><span class="sxs-lookup"><span data-stu-id="611e8-143">String</span></span>                             | <span data-ttu-id="611e8-144">Миддлие имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="611e8-144">Middlie Name of the user.</span></span>                                                                                    |
|<span data-ttu-id="611e8-145">прозвищ</span><span class="sxs-lookup"><span data-stu-id="611e8-145">nickname</span></span>      |<span data-ttu-id="611e8-146">String</span><span class="sxs-lookup"><span data-stu-id="611e8-146">String</span></span>                             | <span data-ttu-id="611e8-147">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="611e8-147">Nickname of the user.</span></span>                                                                                        |
|<span data-ttu-id="611e8-148">произношение</span><span class="sxs-lookup"><span data-stu-id="611e8-148">pronunciation</span></span> |[<span data-ttu-id="611e8-149">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="611e8-149">yomiPersonName</span></span>](yomipersonname.md)| <span data-ttu-id="611e8-150">Руководство по произношению имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="611e8-150">Guidance on how to pronounce the users name.</span></span>                                                                 |
|<span data-ttu-id="611e8-151">суффикс</span><span class="sxs-lookup"><span data-stu-id="611e8-151">suffix</span></span>        |<span data-ttu-id="611e8-152">String</span><span class="sxs-lookup"><span data-stu-id="611e8-152">String</span></span>                             | <span data-ttu-id="611e8-153">Обозначения, используемые после имени пользователя (например, "доктор").</span><span class="sxs-lookup"><span data-stu-id="611e8-153">Designators used after the users name (eg: PhD.)</span></span>                                                             |
|<span data-ttu-id="611e8-154">title</span><span class="sxs-lookup"><span data-stu-id="611e8-154">title</span></span>         |<span data-ttu-id="611e8-155">String</span><span class="sxs-lookup"><span data-stu-id="611e8-155">String</span></span>                             | <span data-ttu-id="611e8-156">Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).</span><span class="sxs-lookup"><span data-stu-id="611e8-156">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="611e8-157">Связи</span><span class="sxs-lookup"><span data-stu-id="611e8-157">Relationships</span></span>

<span data-ttu-id="611e8-158">Нет</span><span class="sxs-lookup"><span data-stu-id="611e8-158">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="611e8-159">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="611e8-159">JSON representation</span></span>

<span data-ttu-id="611e8-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="611e8-160">The following is a JSON representation of the resource.</span></span>

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