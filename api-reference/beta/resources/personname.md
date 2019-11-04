---
title: Тип ресурса personName
description: Тип ресурса personName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: aad97177a06933d2dd98c5cc94744450197f7dcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939602"
---
# <a name="personname-resource-type"></a><span data-ttu-id="15472-103">Тип ресурса personName</span><span class="sxs-lookup"><span data-stu-id="15472-103">personName resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15472-104">Представляет сведения о расширенных именах, предоставленных пользователем или связанными с их учетной записью.</span><span class="sxs-lookup"><span data-stu-id="15472-104">Represents extended name information provided by the user or which they have associated with their account.</span></span>

<span data-ttu-id="15472-105">Наследуется от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="15472-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="15472-106">Методы</span><span class="sxs-lookup"><span data-stu-id="15472-106">Methods</span></span>

| <span data-ttu-id="15472-107">Метод</span><span class="sxs-lookup"><span data-stu-id="15472-107">Method</span></span>                                     | <span data-ttu-id="15472-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="15472-108">Return Type</span></span>                 | <span data-ttu-id="15472-109">Описание</span><span class="sxs-lookup"><span data-stu-id="15472-109">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="15472-110">Получение personName</span><span class="sxs-lookup"><span data-stu-id="15472-110">Get personName</span></span>](../api/personname-get.md) | [<span data-ttu-id="15472-111">personName</span><span class="sxs-lookup"><span data-stu-id="15472-111">personName</span></span>](personname.md) | <span data-ttu-id="15472-112">Чтение свойств и связей объекта personName.</span><span class="sxs-lookup"><span data-stu-id="15472-112">Read properties and relationships of personName object.</span></span> |
| [<span data-ttu-id="15472-113">Update</span><span class="sxs-lookup"><span data-stu-id="15472-113">Update</span></span>](../api/personname-update.md)      | [<span data-ttu-id="15472-114">personName</span><span class="sxs-lookup"><span data-stu-id="15472-114">personName</span></span>](personname.md) | <span data-ttu-id="15472-115">Обновление объекта personName.</span><span class="sxs-lookup"><span data-stu-id="15472-115">Update personName object.</span></span>                               |
| [<span data-ttu-id="15472-116">Delete</span><span class="sxs-lookup"><span data-stu-id="15472-116">Delete</span></span>](../api/personname-delete.md)      | <span data-ttu-id="15472-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="15472-117">None</span></span>                        | <span data-ttu-id="15472-118">Удаление объекта personName.</span><span class="sxs-lookup"><span data-stu-id="15472-118">Delete personName object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="15472-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="15472-119">Properties</span></span>

| <span data-ttu-id="15472-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="15472-120">Property</span></span>     | <span data-ttu-id="15472-121">Тип</span><span class="sxs-lookup"><span data-stu-id="15472-121">Type</span></span>                              | <span data-ttu-id="15472-122">Описание</span><span class="sxs-lookup"><span data-stu-id="15472-122">Description</span></span> |
|:-------------|:----------------------------------|:------------|
|<span data-ttu-id="15472-123">displayName</span><span class="sxs-lookup"><span data-stu-id="15472-123">displayName</span></span>   |<span data-ttu-id="15472-124">Строка</span><span class="sxs-lookup"><span data-stu-id="15472-124">String</span></span>                             | <span data-ttu-id="15472-125">Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства.</span><span class="sxs-lookup"><span data-stu-id="15472-125">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span> |
|<span data-ttu-id="15472-126">первыми</span><span class="sxs-lookup"><span data-stu-id="15472-126">first</span></span>         |<span data-ttu-id="15472-127">Строка</span><span class="sxs-lookup"><span data-stu-id="15472-127">String</span></span>                             | <span data-ttu-id="15472-128">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="15472-128">First Name of the user.</span></span>                                                                                      |
|<span data-ttu-id="15472-129">initials</span><span class="sxs-lookup"><span data-stu-id="15472-129">initials</span></span>      |<span data-ttu-id="15472-130">String</span><span class="sxs-lookup"><span data-stu-id="15472-130">String</span></span>                             | <span data-ttu-id="15472-131">Инициалы пользователя.</span><span class="sxs-lookup"><span data-stu-id="15472-131">Initials of the user.</span></span>                                                                                        |
|<span data-ttu-id="15472-132">лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="15472-132">languageTag</span></span>   |<span data-ttu-id="15472-133">Строка</span><span class="sxs-lookup"><span data-stu-id="15472-133">String</span></span>                             | <span data-ttu-id="15472-134">Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.</span><span class="sxs-lookup"><span data-stu-id="15472-134">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>                        |
|<span data-ttu-id="15472-135">Фамили</span><span class="sxs-lookup"><span data-stu-id="15472-135">last</span></span>          |<span data-ttu-id="15472-136">Строка</span><span class="sxs-lookup"><span data-stu-id="15472-136">String</span></span>                             | <span data-ttu-id="15472-137">Фамилия пользователя.</span><span class="sxs-lookup"><span data-stu-id="15472-137">Last Name of the user.</span></span>                                                                                       |
|<span data-ttu-id="15472-138">маиден</span><span class="sxs-lookup"><span data-stu-id="15472-138">maiden</span></span>        |<span data-ttu-id="15472-139">Строка</span><span class="sxs-lookup"><span data-stu-id="15472-139">String</span></span>                             | <span data-ttu-id="15472-140">Маиден имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="15472-140">Maiden Name of the user.</span></span>                                                                                     |
|<span data-ttu-id="15472-141">назван</span><span class="sxs-lookup"><span data-stu-id="15472-141">middle</span></span>        |<span data-ttu-id="15472-142">Строка</span><span class="sxs-lookup"><span data-stu-id="15472-142">String</span></span>                             | <span data-ttu-id="15472-143">Миддлие имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="15472-143">Middlie Name of the user.</span></span>                                                                                    | 
|<span data-ttu-id="15472-144">прозвищ</span><span class="sxs-lookup"><span data-stu-id="15472-144">nickname</span></span>      |<span data-ttu-id="15472-145">Строка</span><span class="sxs-lookup"><span data-stu-id="15472-145">String</span></span>                             | <span data-ttu-id="15472-146">Псевдоним пользователя.</span><span class="sxs-lookup"><span data-stu-id="15472-146">Nickname of the user.</span></span>                                                                                        |
|<span data-ttu-id="15472-147">произношение</span><span class="sxs-lookup"><span data-stu-id="15472-147">pronunciation</span></span> |[<span data-ttu-id="15472-148">йомиперсоннаме</span><span class="sxs-lookup"><span data-stu-id="15472-148">yomiPersonName</span></span>](yomipersonname.md)| <span data-ttu-id="15472-149">Руководство по произношению имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="15472-149">Guidance on how to pronounce the users name.</span></span>                                                                 |
|<span data-ttu-id="15472-150">суффикс</span><span class="sxs-lookup"><span data-stu-id="15472-150">suffix</span></span>        |<span data-ttu-id="15472-151">Строка</span><span class="sxs-lookup"><span data-stu-id="15472-151">String</span></span>                             | <span data-ttu-id="15472-152">Обозначения, используемые после имени пользователя (например, "доктор").</span><span class="sxs-lookup"><span data-stu-id="15472-152">Designators used after the users name (eg: PhD.)</span></span>                                                             |
|<span data-ttu-id="15472-153">title</span><span class="sxs-lookup"><span data-stu-id="15472-153">title</span></span>         |<span data-ttu-id="15472-154">String</span><span class="sxs-lookup"><span data-stu-id="15472-154">String</span></span>                             | <span data-ttu-id="15472-155">Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).</span><span class="sxs-lookup"><span data-stu-id="15472-155">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="15472-156">Связи</span><span class="sxs-lookup"><span data-stu-id="15472-156">Relationships</span></span>

<span data-ttu-id="15472-157">Нет</span><span class="sxs-lookup"><span data-stu-id="15472-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15472-158">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15472-158">JSON representation</span></span>

<span data-ttu-id="15472-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15472-159">The following is a JSON representation of the resource.</span></span>

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