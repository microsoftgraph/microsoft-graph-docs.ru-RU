---
title: Обновление profileCardProperty
description: Обновление свойств объекта profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 53d95deee5be591745e62d7c41b2ab232b3b19d8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52036690"
---
# <a name="update-profilecardproperty"></a><span data-ttu-id="84de4-103">Обновление profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="84de4-103">Update profileCardProperty</span></span>

<span data-ttu-id="84de4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84de4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84de4-105">Обновление свойств объекта [profileCardProperty,](../resources/profilecardproperty.md) определенного свойством **directoryPropertyName.**</span><span class="sxs-lookup"><span data-stu-id="84de4-105">Update the properties of a [profileCardProperty](../resources/profilecardproperty.md) object, identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="84de4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84de4-106">Permissions</span></span>

<span data-ttu-id="84de4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84de4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="84de4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84de4-109">Permission type</span></span>                        | <span data-ttu-id="84de4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84de4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="84de4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84de4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="84de4-112">User.ReadWrite, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84de4-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="84de4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84de4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84de4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84de4-114">Not supported.</span></span>                              |
| <span data-ttu-id="84de4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84de4-115">Application</span></span>                            | <span data-ttu-id="84de4-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="84de4-116">Not supported.</span></span>                              |

><span data-ttu-id="84de4-117">**Примечание:** Использование делегирования разрешений для этой операции требует от пользователя, вписаного, роли администратора клиента или глобального администратора.</span><span class="sxs-lookup"><span data-stu-id="84de4-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="84de4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84de4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="84de4-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="84de4-119">Request headers</span></span>

| <span data-ttu-id="84de4-120">Имя</span><span class="sxs-lookup"><span data-stu-id="84de4-120">Name</span></span>       | <span data-ttu-id="84de4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="84de4-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="84de4-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="84de4-122">Authorization</span></span> | <span data-ttu-id="84de4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84de4-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="84de4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="84de4-125">Content-Type</span></span>  | <span data-ttu-id="84de4-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84de4-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="84de4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="84de4-128">Request body</span></span>

<span data-ttu-id="84de4-129">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="84de4-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="84de4-130">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="84de4-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="84de4-131">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="84de4-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="84de4-132">Свойство</span><span class="sxs-lookup"><span data-stu-id="84de4-132">Property</span></span>     | <span data-ttu-id="84de4-133">Тип</span><span class="sxs-lookup"><span data-stu-id="84de4-133">Type</span></span>        | <span data-ttu-id="84de4-134">Описание</span><span class="sxs-lookup"><span data-stu-id="84de4-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84de4-135">аннотации</span><span class="sxs-lookup"><span data-stu-id="84de4-135">annotations</span></span>|<span data-ttu-id="84de4-136">коллекция profileCardAnnotation</span><span class="sxs-lookup"><span data-stu-id="84de4-136">profileCardAnnotation collection</span></span>| <span data-ttu-id="84de4-137">Содержит любые альтернативные или локализованные метки, которые администратор выбрал для указания.</span><span class="sxs-lookup"><span data-stu-id="84de4-137">Contains any alternative or localized labels an administrator has chosen to specify.</span></span>|
|<span data-ttu-id="84de4-138">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="84de4-138">directoryPropertyName</span></span>|<span data-ttu-id="84de4-139">String</span><span class="sxs-lookup"><span data-stu-id="84de4-139">String</span></span>|<span data-ttu-id="84de4-140">Содержит имя свойства каталога, которое должно всплыть на карточке профиля.</span><span class="sxs-lookup"><span data-stu-id="84de4-140">Contains the name of the directory property which is intended to surface on the profile card.</span></span> |

## <a name="response"></a><span data-ttu-id="84de4-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="84de4-141">Response</span></span>

<span data-ttu-id="84de4-142">В случае успешной работы этот метод возвращает код отклика и обновленный `200 OK` [объект profileCardProperty](../resources/profilecardproperty.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="84de4-142">If successful, this method returns a `200 OK` response code and an updated [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="84de4-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="84de4-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="84de4-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="84de4-144">Request</span></span>

<span data-ttu-id="84de4-145">В следующем примере добавляется локализованная метка "Senter Kostnads" для локального "no-NB".</span><span class="sxs-lookup"><span data-stu-id="84de4-145">The following example adds a localized label "Kostnads Senter" for the locale "no-NB".</span></span>

# <a name="http"></a>[<span data-ttu-id="84de4-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="84de4-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilecardproperty"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/CustomAttribute1
Content-type: application/json

{
  "annotations": [
    {
      "localizations": [
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="84de4-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84de4-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="84de4-148">C#</span><span class="sxs-lookup"><span data-stu-id="84de4-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="84de4-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="84de4-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="84de4-150">Java</span><span class="sxs-lookup"><span data-stu-id="84de4-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilecardproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="84de4-151">Отклик</span><span class="sxs-lookup"><span data-stu-id="84de4-151">Response</span></span>

<span data-ttu-id="84de4-152">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="84de4-152">The following is an example of the response.</span></span>

> <span data-ttu-id="84de4-153">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="84de4-153">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        },
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilecardproperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


