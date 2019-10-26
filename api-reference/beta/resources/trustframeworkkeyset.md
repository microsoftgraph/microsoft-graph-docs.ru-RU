---
title: Тип ресурса Трустфрамеворккэйсет
description: Представляет ключи набора ключей и политики для инфраструктуры доверия.
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8ecc644e09f7e57433c263e883513dfbb6294465
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734678"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="014e7-103">Тип ресурса Трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="014e7-103">trustFrameworkKeySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="014e7-104">Представляет ключи набора ключей и политики для инфраструктуры доверия.</span><span class="sxs-lookup"><span data-stu-id="014e7-104">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="014e7-105">В платформе удостоверений хранятся секреты, которые можно использовать в политиках.</span><span class="sxs-lookup"><span data-stu-id="014e7-105">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="014e7-106">Секреты могут представлять собой пароли, сертификаты и другие файлы.</span><span class="sxs-lookup"><span data-stu-id="014e7-106">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="014e7-107">В портале эти сущности отображаются как `Policy keys`.</span><span class="sxs-lookup"><span data-stu-id="014e7-107">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="014e7-108">Платформа удостоверений использует стандарт JSON Web Key (ЖВК) для кэйсетс.</span><span class="sxs-lookup"><span data-stu-id="014e7-108">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="014e7-109">Эта сущность соответствует формату, указанному в [RFC 7517 в разделе 5](https://tools.ietf.org/html/rfc7517#section-5).</span><span class="sxs-lookup"><span data-stu-id="014e7-109">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="014e7-110">Методы</span><span class="sxs-lookup"><span data-stu-id="014e7-110">Methods</span></span>

| <span data-ttu-id="014e7-111">Метод</span><span class="sxs-lookup"><span data-stu-id="014e7-111">Method</span></span>       | <span data-ttu-id="014e7-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="014e7-112">Return Type</span></span> | <span data-ttu-id="014e7-113">Описание</span><span class="sxs-lookup"><span data-stu-id="014e7-113">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="014e7-114">Получение</span><span class="sxs-lookup"><span data-stu-id="014e7-114">Get</span></span>](../api/trustframeworkkeyset-get.md) | [<span data-ttu-id="014e7-115">трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="014e7-115">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="014e7-116">Чтение свойств и связей объекта Трустфрамеворккэйсет.</span><span class="sxs-lookup"><span data-stu-id="014e7-116">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| <span data-ttu-id="014e7-117">[обновление](../api/trustframeworkkeyset-update.md).</span><span class="sxs-lookup"><span data-stu-id="014e7-117">[Update](../api/trustframeworkkeyset-update.md)</span></span> | [<span data-ttu-id="014e7-118">трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="014e7-118">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="014e7-119">Обновление объекта Трустфрамеворккэйсет.</span><span class="sxs-lookup"><span data-stu-id="014e7-119">Update trustFrameworkKeySet object.</span></span> |
| <span data-ttu-id="014e7-120">[удаление](../api/trustframeworkkeyset-delete.md);</span><span class="sxs-lookup"><span data-stu-id="014e7-120">[Delete](../api/trustframeworkkeyset-delete.md)</span></span> | <span data-ttu-id="014e7-121">Нет</span><span class="sxs-lookup"><span data-stu-id="014e7-121">None</span></span> | <span data-ttu-id="014e7-122">Удаление объекта Трустфрамеворккэйсет.</span><span class="sxs-lookup"><span data-stu-id="014e7-122">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="014e7-123">женератекэй</span><span class="sxs-lookup"><span data-stu-id="014e7-123">Generatekey</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="014e7-124">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="014e7-124">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="014e7-125">Создание ключа в наборе ключей.</span><span class="sxs-lookup"><span data-stu-id="014e7-125">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="014e7-126">жетактивекэй</span><span class="sxs-lookup"><span data-stu-id="014e7-126">Getactivekey</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="014e7-127">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="014e7-127">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="014e7-128">Получить активный в данный момент ключ в наборе ключей.</span><span class="sxs-lookup"><span data-stu-id="014e7-128">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="014e7-129">уплоадцертификате</span><span class="sxs-lookup"><span data-stu-id="014e7-129">Uploadcertificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="014e7-130">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="014e7-130">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="014e7-131">Отправьте сертификат X. 509.</span><span class="sxs-lookup"><span data-stu-id="014e7-131">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="014e7-132">Uploadpkcs12</span><span class="sxs-lookup"><span data-stu-id="014e7-132">Uploadpkcs12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="014e7-133">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="014e7-133">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="014e7-134">Отправьте сертификат формата PKCS12.</span><span class="sxs-lookup"><span data-stu-id="014e7-134">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="014e7-135">уплоадсекрет</span><span class="sxs-lookup"><span data-stu-id="014e7-135">Uploadsecret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="014e7-136">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="014e7-136">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="014e7-137">Отправка секрета на основе строки.</span><span class="sxs-lookup"><span data-stu-id="014e7-137">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="014e7-138">Свойства</span><span class="sxs-lookup"><span data-stu-id="014e7-138">Properties</span></span>

| <span data-ttu-id="014e7-139">Свойство</span><span class="sxs-lookup"><span data-stu-id="014e7-139">Property</span></span>     | <span data-ttu-id="014e7-140">Тип</span><span class="sxs-lookup"><span data-stu-id="014e7-140">Type</span></span>        | <span data-ttu-id="014e7-141">Описание</span><span class="sxs-lookup"><span data-stu-id="014e7-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="014e7-142">id</span><span class="sxs-lookup"><span data-stu-id="014e7-142">id</span></span>|<span data-ttu-id="014e7-143">String</span><span class="sxs-lookup"><span data-stu-id="014e7-143">String</span></span>| <span data-ttu-id="014e7-144">Уникальный идентификатор набора ключей трустфрамеворк</span><span class="sxs-lookup"><span data-stu-id="014e7-144">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="014e7-145">переключен</span><span class="sxs-lookup"><span data-stu-id="014e7-145">keys</span></span>|<span data-ttu-id="014e7-146">Коллекция [трустфрамеворккэй](trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="014e7-146">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="014e7-147">Коллекция ключей.</span><span class="sxs-lookup"><span data-stu-id="014e7-147">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="014e7-148">Связи</span><span class="sxs-lookup"><span data-stu-id="014e7-148">Relationships</span></span>

<span data-ttu-id="014e7-149">Нет</span><span class="sxs-lookup"><span data-stu-id="014e7-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="014e7-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="014e7-150">JSON representation</span></span>

<span data-ttu-id="014e7-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="014e7-151">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.trustFrameworkKeySet",
  "baseType": "",
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
