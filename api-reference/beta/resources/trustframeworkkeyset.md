---
title: Тип ресурса trustFrameworkKeySet
description: Представляет набор ключей и ключи политики для структуры доверия.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4223681a11ff11b8ea75b165247b5269d1a6cf84
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159859"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="adff9-103">Тип ресурса trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="adff9-103">trustFrameworkKeySet resource type</span></span>

<span data-ttu-id="adff9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adff9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adff9-105">Представляет набор ключей и ключи политики для структуры доверия.</span><span class="sxs-lookup"><span data-stu-id="adff9-105">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="adff9-106">В базе identity Experience framework хранится секрет, который можно использовать в политиках.</span><span class="sxs-lookup"><span data-stu-id="adff9-106">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="adff9-107">Секреты могут быть паролями, сертификатами или другими файлами.</span><span class="sxs-lookup"><span data-stu-id="adff9-107">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="adff9-108">На портале эти сущности показаны как `Policy keys` .</span><span class="sxs-lookup"><span data-stu-id="adff9-108">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="adff9-109">В структуре identity Experience используется стандарт JSON Web Key (JWK) для ключей.</span><span class="sxs-lookup"><span data-stu-id="adff9-109">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="adff9-110">Эта сущность следует формату, указанному в разделе [5 RFC 7517.](https://tools.ietf.org/html/rfc7517#section-5)</span><span class="sxs-lookup"><span data-stu-id="adff9-110">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="adff9-111">Методы</span><span class="sxs-lookup"><span data-stu-id="adff9-111">Methods</span></span>

| <span data-ttu-id="adff9-112">Метод</span><span class="sxs-lookup"><span data-stu-id="adff9-112">Method</span></span>       | <span data-ttu-id="adff9-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="adff9-113">Return Type</span></span> | <span data-ttu-id="adff9-114">Описание</span><span class="sxs-lookup"><span data-stu-id="adff9-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="adff9-115">Список</span><span class="sxs-lookup"><span data-stu-id="adff9-115">List</span></span>](../api/trustframework-list-keysets.md) | <span data-ttu-id="adff9-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Коллекция</span><span class="sxs-lookup"><span data-stu-id="adff9-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Collection</span></span> | <span data-ttu-id="adff9-117">Список trustFrameworkKeySets.</span><span class="sxs-lookup"><span data-stu-id="adff9-117">List trustFrameworkKeySets.</span></span> |
| [<span data-ttu-id="adff9-118">Создание</span><span class="sxs-lookup"><span data-stu-id="adff9-118">Create</span></span>](../api/trustframework-post-keysets.md) | [<span data-ttu-id="adff9-119">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="adff9-119">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="adff9-120">Создание trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="adff9-120">Create  trustFrameworkKeySet.</span></span> |
| [<span data-ttu-id="adff9-121">Получение</span><span class="sxs-lookup"><span data-stu-id="adff9-121">Get</span></span>](../api/trustframeworkkeyset-get.md) | [<span data-ttu-id="adff9-122">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="adff9-122">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="adff9-123">Чтение свойств и связей объекта trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="adff9-123">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="adff9-124">Обновление</span><span class="sxs-lookup"><span data-stu-id="adff9-124">Update</span></span>](../api/trustframeworkkeyset-update.md) | [<span data-ttu-id="adff9-125">trustFrameworkKeySet</span><span class="sxs-lookup"><span data-stu-id="adff9-125">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="adff9-126">Обновление объекта trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="adff9-126">Update trustFrameworkKeySet object.</span></span> |
| <span data-ttu-id="adff9-127">[удаление](../api/trustframeworkkeyset-delete.md);</span><span class="sxs-lookup"><span data-stu-id="adff9-127">[Delete](../api/trustframeworkkeyset-delete.md)</span></span> | <span data-ttu-id="adff9-128">Нет</span><span class="sxs-lookup"><span data-stu-id="adff9-128">None</span></span> | <span data-ttu-id="adff9-129">Удаление объекта trustFrameworkKeySet.</span><span class="sxs-lookup"><span data-stu-id="adff9-129">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="adff9-130">Создание ключа</span><span class="sxs-lookup"><span data-stu-id="adff9-130">Generate key</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="adff9-131">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="adff9-131">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="adff9-132">Создание ключа в наборе ключей.</span><span class="sxs-lookup"><span data-stu-id="adff9-132">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="adff9-133">Получить активный ключ</span><span class="sxs-lookup"><span data-stu-id="adff9-133">Get active key</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="adff9-134">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="adff9-134">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="adff9-135">Получите текущий активный ключ в наборе ключей.</span><span class="sxs-lookup"><span data-stu-id="adff9-135">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="adff9-136">Отправка сертификата</span><span class="sxs-lookup"><span data-stu-id="adff9-136">Upload certificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="adff9-137">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="adff9-137">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="adff9-138">Отправка сертификата X.509.</span><span class="sxs-lookup"><span data-stu-id="adff9-138">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="adff9-139">Отправка PKCS12</span><span class="sxs-lookup"><span data-stu-id="adff9-139">Upload PKCS12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="adff9-140">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="adff9-140">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="adff9-141">Отправка сертификата формата PKCS12.</span><span class="sxs-lookup"><span data-stu-id="adff9-141">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="adff9-142">Секрет отправки</span><span class="sxs-lookup"><span data-stu-id="adff9-142">Upload secret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="adff9-143">trustFrameworkKey</span><span class="sxs-lookup"><span data-stu-id="adff9-143">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="adff9-144">Отправка секрета на основе строки.</span><span class="sxs-lookup"><span data-stu-id="adff9-144">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="adff9-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="adff9-145">Properties</span></span>

| <span data-ttu-id="adff9-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="adff9-146">Property</span></span>     | <span data-ttu-id="adff9-147">Тип</span><span class="sxs-lookup"><span data-stu-id="adff9-147">Type</span></span>        | <span data-ttu-id="adff9-148">Описание</span><span class="sxs-lookup"><span data-stu-id="adff9-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="adff9-149">id</span><span class="sxs-lookup"><span data-stu-id="adff9-149">id</span></span>|<span data-ttu-id="adff9-150">String</span><span class="sxs-lookup"><span data-stu-id="adff9-150">String</span></span>| <span data-ttu-id="adff9-151">Уникальный идентификатор наборов ключей инфраструктуры доверия</span><span class="sxs-lookup"><span data-stu-id="adff9-151">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="adff9-152">keys</span><span class="sxs-lookup"><span data-stu-id="adff9-152">keys</span></span>|<span data-ttu-id="adff9-153">[Коллекция trustFrameworkKey](trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="adff9-153">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="adff9-154">Коллекция ключей.</span><span class="sxs-lookup"><span data-stu-id="adff9-154">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="adff9-155">Связи</span><span class="sxs-lookup"><span data-stu-id="adff9-155">Relationships</span></span>

<span data-ttu-id="adff9-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="adff9-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="adff9-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="adff9-157">JSON representation</span></span>

<span data-ttu-id="adff9-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="adff9-158">The following is a JSON representation of the resource.</span></span>

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


