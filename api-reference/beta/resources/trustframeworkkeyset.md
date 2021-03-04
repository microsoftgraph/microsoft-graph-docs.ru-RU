---
title: тип ресурса trustFrameworkKeySet
description: Представляет набор ключей и ключей политики для фреймворка доверия.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4bd20bd3b9df4656a3bbc73a52511d64ad463bf5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442770"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="5c933-103">тип ресурса trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5c933-103">trustFrameworkKeySet resource type</span></span>

<span data-ttu-id="5c933-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c933-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c933-105">Представляет набор ключей и ключей политики для фреймворка доверия.</span><span class="sxs-lookup"><span data-stu-id="5c933-105">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="5c933-106">В фреймворках Identity Experience хранится секрет, который можно использовать в политиках.</span><span class="sxs-lookup"><span data-stu-id="5c933-106">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="5c933-107">Секретами могут быть пароли, сертификаты или другие файлы.</span><span class="sxs-lookup"><span data-stu-id="5c933-107">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="5c933-108">На портале эти сущности показаны как `Policy keys` .</span><span class="sxs-lookup"><span data-stu-id="5c933-108">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="5c933-109">В рамках "Опыт удостоверений" используется стандарт веб-ключа JSON (JWK) для клавиш.</span><span class="sxs-lookup"><span data-stu-id="5c933-109">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="5c933-110">Эта сущность следует формату, указанному в [разделе 5 RFC 7517.](https://tools.ietf.org/html/rfc7517#section-5)</span><span class="sxs-lookup"><span data-stu-id="5c933-110">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="5c933-111">Методы</span><span class="sxs-lookup"><span data-stu-id="5c933-111">Methods</span></span>

| <span data-ttu-id="5c933-112">Метод</span><span class="sxs-lookup"><span data-stu-id="5c933-112">Method</span></span>       | <span data-ttu-id="5c933-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5c933-113">Return Type</span></span> | <span data-ttu-id="5c933-114">Описание</span><span class="sxs-lookup"><span data-stu-id="5c933-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5c933-115">Список</span><span class="sxs-lookup"><span data-stu-id="5c933-115">List</span></span>](../api/trustframework-list-keysets.md) | <span data-ttu-id="5c933-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Коллекция</span><span class="sxs-lookup"><span data-stu-id="5c933-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Collection</span></span> | <span data-ttu-id="5c933-117">Список trustFrameworkKeySets.</span><span class="sxs-lookup"><span data-stu-id="5c933-117">List trustFrameworkKeySets.</span></span> |
| [<span data-ttu-id="5c933-118">Создание</span><span class="sxs-lookup"><span data-stu-id="5c933-118">Create</span></span>](../api/trustframework-post-keysets.md) | [<span data-ttu-id="5c933-119">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5c933-119">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="5c933-120">Создание trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="5c933-120">Create  trustFrameworkKeySet.</span></span> |
| <span data-ttu-id="5c933-121">[получение](../api/trustframeworkkeyset-get.md);</span><span class="sxs-lookup"><span data-stu-id="5c933-121">[Get](../api/trustframeworkkeyset-get.md)</span></span> | [<span data-ttu-id="5c933-122">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5c933-122">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="5c933-123">Чтение свойств и связей объекта trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="5c933-123">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="5c933-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="5c933-124">Update</span></span>](../api/trustframeworkkeyset-update.md) | [<span data-ttu-id="5c933-125">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="5c933-125">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="5c933-126">Обновление объекта trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="5c933-126">Update trustFrameworkKeySet object.</span></span> |
| <span data-ttu-id="5c933-127">[удаление](../api/trustframeworkkeyset-delete.md);</span><span class="sxs-lookup"><span data-stu-id="5c933-127">[Delete](../api/trustframeworkkeyset-delete.md)</span></span> | <span data-ttu-id="5c933-128">Нет</span><span class="sxs-lookup"><span data-stu-id="5c933-128">None</span></span> | <span data-ttu-id="5c933-129">Удаление объекта trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="5c933-129">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="5c933-130">Создание ключа</span><span class="sxs-lookup"><span data-stu-id="5c933-130">Generate key</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="5c933-131">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5c933-131">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5c933-132">Создание ключа в наборе ключей.</span><span class="sxs-lookup"><span data-stu-id="5c933-132">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="5c933-133">Получить активный ключ</span><span class="sxs-lookup"><span data-stu-id="5c933-133">Get active key</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="5c933-134">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5c933-134">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5c933-135">Получите активный ключ в наборе ключей.</span><span class="sxs-lookup"><span data-stu-id="5c933-135">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="5c933-136">Сертификат загрузки</span><span class="sxs-lookup"><span data-stu-id="5c933-136">Upload certificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="5c933-137">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5c933-137">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5c933-138">Загрузите сертификат X.509.</span><span class="sxs-lookup"><span data-stu-id="5c933-138">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="5c933-139">Загрузка PKCS12</span><span class="sxs-lookup"><span data-stu-id="5c933-139">Upload PKCS12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="5c933-140">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5c933-140">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5c933-141">Загрузите сертификат формата PKCS12.</span><span class="sxs-lookup"><span data-stu-id="5c933-141">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="5c933-142">Отправка секрета</span><span class="sxs-lookup"><span data-stu-id="5c933-142">Upload secret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="5c933-143">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="5c933-143">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="5c933-144">Загрузите секрет на основе строки.</span><span class="sxs-lookup"><span data-stu-id="5c933-144">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="5c933-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c933-145">Properties</span></span>

| <span data-ttu-id="5c933-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c933-146">Property</span></span>     | <span data-ttu-id="5c933-147">Тип</span><span class="sxs-lookup"><span data-stu-id="5c933-147">Type</span></span>        | <span data-ttu-id="5c933-148">Описание</span><span class="sxs-lookup"><span data-stu-id="5c933-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5c933-149">id</span><span class="sxs-lookup"><span data-stu-id="5c933-149">id</span></span>|<span data-ttu-id="5c933-150">String</span><span class="sxs-lookup"><span data-stu-id="5c933-150">String</span></span>| <span data-ttu-id="5c933-151">Уникальный идентификатор наборов ключей trustframework</span><span class="sxs-lookup"><span data-stu-id="5c933-151">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="5c933-152">клавиши</span><span class="sxs-lookup"><span data-stu-id="5c933-152">keys</span></span>|<span data-ttu-id="5c933-153">[коллекция trustFrameworkKey](trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="5c933-153">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="5c933-154">Коллекция ключей.</span><span class="sxs-lookup"><span data-stu-id="5c933-154">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5c933-155">Связи</span><span class="sxs-lookup"><span data-stu-id="5c933-155">Relationships</span></span>

<span data-ttu-id="5c933-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5c933-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c933-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5c933-157">JSON representation</span></span>

<span data-ttu-id="5c933-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c933-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "keys": [{"@odata.type": "microsoft.graph.trustFrameworkKey"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


