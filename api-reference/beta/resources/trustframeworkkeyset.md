---
title: Тип ресурса Трустфрамеворккэйсет
description: Представляет ключи набора ключей и политики для инфраструктуры доверия.
localization_priority: Normal
author: Nickgmicrosoft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0784bffd1682f59e94d728c2311ffaaa01681c5
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218053"
---
# <a name="trustframeworkkeyset-resource-type"></a><span data-ttu-id="f7f9f-103">Тип ресурса Трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="f7f9f-103">trustFrameworkKeySet resource type</span></span>

<span data-ttu-id="f7f9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7f9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7f9f-105">Представляет ключи набора ключей и политики для инфраструктуры доверия.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-105">Represents a trust framework keyset/policy keys.</span></span> <span data-ttu-id="f7f9f-106">В платформе удостоверений хранятся секреты, которые можно использовать в политиках.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-106">The Identity Experience framework stores the secrets, which can be used in the policies.</span></span> <span data-ttu-id="f7f9f-107">Секреты могут представлять собой пароли, сертификаты и другие файлы.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-107">The secrets can be passwords, certificates, or other files.</span></span> <span data-ttu-id="f7f9f-108">В портале эти сущности отображаются как `Policy keys`.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-108">In the portal, these entities are shown as `Policy keys`.</span></span> <span data-ttu-id="f7f9f-109">Платформа удостоверений использует стандарт JSON Web Key (ЖВК) для кэйсетс.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-109">The Identity Experience framework uses the JSON Web Key (JWK) standard for the keysets.</span></span> <span data-ttu-id="f7f9f-110">Эта сущность соответствует формату, указанному в [RFC 7517 в разделе 5](https://tools.ietf.org/html/rfc7517#section-5).</span><span class="sxs-lookup"><span data-stu-id="f7f9f-110">This entity follows the format specified in [RFC 7517 Section 5](https://tools.ietf.org/html/rfc7517#section-5).</span></span>

## <a name="methods"></a><span data-ttu-id="f7f9f-111">Методы</span><span class="sxs-lookup"><span data-stu-id="f7f9f-111">Methods</span></span>

| <span data-ttu-id="f7f9f-112">Метод</span><span class="sxs-lookup"><span data-stu-id="f7f9f-112">Method</span></span>       | <span data-ttu-id="f7f9f-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f7f9f-113">Return Type</span></span> | <span data-ttu-id="f7f9f-114">Описание</span><span class="sxs-lookup"><span data-stu-id="f7f9f-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f7f9f-115">List</span><span class="sxs-lookup"><span data-stu-id="f7f9f-115">List</span></span>](../api/trustframework-list-keysets.md) | <span data-ttu-id="f7f9f-116">[трустфрамеворккэйсет](trustframeworkkeyset.md) Семейства</span><span class="sxs-lookup"><span data-stu-id="f7f9f-116">[trustFrameworkKeySet](trustframeworkkeyset.md) Collection</span></span> | <span data-ttu-id="f7f9f-117">Список Трустфрамеворккэйсетс.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-117">List trustFrameworkKeySets.</span></span> |
| <span data-ttu-id="f7f9f-118">[создание](../api/trustframework-post-keysets.md);</span><span class="sxs-lookup"><span data-stu-id="f7f9f-118">[Create](../api/trustframework-post-keysets.md)</span></span> | [<span data-ttu-id="f7f9f-119">трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="f7f9f-119">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="f7f9f-120">Создайте Трустфрамеворккэйсет.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-120">Create  trustFrameworkKeySet.</span></span> |
| <span data-ttu-id="f7f9f-121">[получение](../api/trustframeworkkeyset-get.md);</span><span class="sxs-lookup"><span data-stu-id="f7f9f-121">[Get](../api/trustframeworkkeyset-get.md)</span></span> | [<span data-ttu-id="f7f9f-122">трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="f7f9f-122">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="f7f9f-123">Чтение свойств и связей объекта Трустфрамеворккэйсет.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-123">Read properties and relationships of trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="f7f9f-124">Update</span><span class="sxs-lookup"><span data-stu-id="f7f9f-124">Update</span></span>](../api/trustframeworkkeyset-update.md) | [<span data-ttu-id="f7f9f-125">трустфрамеворккэйсет</span><span class="sxs-lookup"><span data-stu-id="f7f9f-125">trustFrameworkKeySet</span></span>](trustframeworkkeyset.md) | <span data-ttu-id="f7f9f-126">Обновление объекта Трустфрамеворккэйсет.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-126">Update trustFrameworkKeySet object.</span></span> |
| [<span data-ttu-id="f7f9f-127">Удаление</span><span class="sxs-lookup"><span data-stu-id="f7f9f-127">Delete</span></span>](../api/trustframeworkkeyset-delete.md) | <span data-ttu-id="f7f9f-128">Нет</span><span class="sxs-lookup"><span data-stu-id="f7f9f-128">None</span></span> | <span data-ttu-id="f7f9f-129">Удаление объекта Трустфрамеворккэйсет.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-129">Delete trustFrameworkKeySet object.</span></span> |
|[<span data-ttu-id="f7f9f-130">Создание ключа</span><span class="sxs-lookup"><span data-stu-id="f7f9f-130">Generate key</span></span>](../api/trustframeworkkeyset-generatekey.md)|[<span data-ttu-id="f7f9f-131">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="f7f9f-131">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="f7f9f-132">Создание ключа в наборе ключей.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-132">Generate a key in keyset.</span></span> |
|[<span data-ttu-id="f7f9f-133">Получение активного ключа</span><span class="sxs-lookup"><span data-stu-id="f7f9f-133">Get active key</span></span>](../api/trustframeworkkeyset-getactivekey.md)|[<span data-ttu-id="f7f9f-134">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="f7f9f-134">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="f7f9f-135">Получить активный в данный момент ключ в наборе ключей.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-135">Get currently active key in the keyset.</span></span> |
|[<span data-ttu-id="f7f9f-136">Отправка сертификата</span><span class="sxs-lookup"><span data-stu-id="f7f9f-136">Upload certificate</span></span>](../api/trustframeworkkeyset-uploadcertificate.md)|[<span data-ttu-id="f7f9f-137">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="f7f9f-137">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="f7f9f-138">Отправьте сертификат X. 509.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-138">Upload a X.509 certificate.</span></span> |
|[<span data-ttu-id="f7f9f-139">Отправка PKCS12</span><span class="sxs-lookup"><span data-stu-id="f7f9f-139">Upload PKCS12</span></span>](../api/trustframeworkkeyset-uploadpkcs12.md)|[<span data-ttu-id="f7f9f-140">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="f7f9f-140">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="f7f9f-141">Отправьте сертификат формата PKCS12.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-141">Upload a PKCS12 format certificate.</span></span> |
|[<span data-ttu-id="f7f9f-142">Отправка секрета</span><span class="sxs-lookup"><span data-stu-id="f7f9f-142">Upload secret</span></span>](../api/trustframeworkkeyset-uploadsecret.md)|[<span data-ttu-id="f7f9f-143">трустфрамеворккэй</span><span class="sxs-lookup"><span data-stu-id="f7f9f-143">trustFrameworkKey</span></span>](trustframeworkkey.md)| <span data-ttu-id="f7f9f-144">Отправка секрета на основе строки.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-144">Upload a string based secret.</span></span> |

## <a name="properties"></a><span data-ttu-id="f7f9f-145">Свойства</span><span class="sxs-lookup"><span data-stu-id="f7f9f-145">Properties</span></span>

| <span data-ttu-id="f7f9f-146">Свойство</span><span class="sxs-lookup"><span data-stu-id="f7f9f-146">Property</span></span>     | <span data-ttu-id="f7f9f-147">Тип</span><span class="sxs-lookup"><span data-stu-id="f7f9f-147">Type</span></span>        | <span data-ttu-id="f7f9f-148">Описание</span><span class="sxs-lookup"><span data-stu-id="f7f9f-148">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f7f9f-149">id</span><span class="sxs-lookup"><span data-stu-id="f7f9f-149">id</span></span>|<span data-ttu-id="f7f9f-150">Строка</span><span class="sxs-lookup"><span data-stu-id="f7f9f-150">String</span></span>| <span data-ttu-id="f7f9f-151">Уникальный идентификатор набора ключей трустфрамеворк</span><span class="sxs-lookup"><span data-stu-id="f7f9f-151">Unique identifier of the trustframework keyset</span></span> |
|<span data-ttu-id="f7f9f-152">переключен</span><span class="sxs-lookup"><span data-stu-id="f7f9f-152">keys</span></span>|<span data-ttu-id="f7f9f-153">Коллекция [трустфрамеворккэй](trustframeworkkey.md)</span><span class="sxs-lookup"><span data-stu-id="f7f9f-153">[trustFrameworkKey](trustframeworkkey.md) collection</span></span>| <span data-ttu-id="f7f9f-154">Коллекция ключей.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-154">A collection of the keys.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f7f9f-155">Отношения</span><span class="sxs-lookup"><span data-stu-id="f7f9f-155">Relationships</span></span>

<span data-ttu-id="f7f9f-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7f9f-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f7f9f-157">JSON representation</span></span>

<span data-ttu-id="f7f9f-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f7f9f-158">The following is a JSON representation of the resource.</span></span>

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
