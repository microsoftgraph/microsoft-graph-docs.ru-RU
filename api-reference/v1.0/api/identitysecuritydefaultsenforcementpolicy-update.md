---
title: Обновление Идентитисекуритидефаултсенфорцементполици
description: Обновление свойств объекта Идентитисекуритидефаултсенфорцементполици.
localization_priority: Normal
author: rohinigoyal1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 57903235da05e04d5fc0e36d65cb491f06442b59
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384729"
---
# <a name="update-identitysecuritydefaultsenforcementpolicy"></a><span data-ttu-id="53f3e-103">Обновление Идентитисекуритидефаултсенфорцементполици</span><span class="sxs-lookup"><span data-stu-id="53f3e-103">Update identitySecurityDefaultsEnforcementPolicy</span></span>

<span data-ttu-id="53f3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53f3e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53f3e-105">Обновление свойств объекта [идентитисекуритидефаултсенфорцементполици](../resources/identitysecuritydefaultsenforcementpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="53f3e-105">Update the properties of an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="53f3e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53f3e-106">Permissions</span></span>

<span data-ttu-id="53f3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53f3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53f3e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53f3e-109">Permission type</span></span>                        | <span data-ttu-id="53f3e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53f3e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="53f3e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53f3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="53f3e-112">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="53f3e-112">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |
| <span data-ttu-id="53f3e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53f3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53f3e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53f3e-114">Not supported.</span></span> |
| <span data-ttu-id="53f3e-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="53f3e-115">Application</span></span>                            | <span data-ttu-id="53f3e-116">Policy. Read. ALL и Policy. ReadWrite. Кондитионалакцесс</span><span class="sxs-lookup"><span data-stu-id="53f3e-116">Policy.Read.All and Policy.ReadWrite.ConditionalAccess</span></span> |

## <a name="http-request"></a><span data-ttu-id="53f3e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53f3e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/identitySecurityDefaultsEnforcementPolicy
```

## <a name="request-headers"></a><span data-ttu-id="53f3e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53f3e-118">Request headers</span></span>

| <span data-ttu-id="53f3e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="53f3e-119">Name</span></span>       | <span data-ttu-id="53f3e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="53f3e-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="53f3e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53f3e-121">Authorization</span></span> | <span data-ttu-id="53f3e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53f3e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="53f3e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="53f3e-124">Content-type</span></span> | <span data-ttu-id="53f3e-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53f3e-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53f3e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53f3e-127">Request body</span></span>

<span data-ttu-id="53f3e-128">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="53f3e-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="53f3e-129">Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств.</span><span class="sxs-lookup"><span data-stu-id="53f3e-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="53f3e-130">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="53f3e-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="53f3e-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="53f3e-131">Property</span></span>     | <span data-ttu-id="53f3e-132">Тип</span><span class="sxs-lookup"><span data-stu-id="53f3e-132">Type</span></span>        | <span data-ttu-id="53f3e-133">Описание</span><span class="sxs-lookup"><span data-stu-id="53f3e-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="53f3e-134">isEnabled</span><span class="sxs-lookup"><span data-stu-id="53f3e-134">isEnabled</span></span>|<span data-ttu-id="53f3e-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="53f3e-135">Boolean</span></span>|<span data-ttu-id="53f3e-136">Если задано значение true, по умолчанию для клиента будет включен параметр безопасности Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="53f3e-136">If set to true, Azure Active Directory security defaults is enabled for the tenant.</span></span>|

## <a name="response"></a><span data-ttu-id="53f3e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="53f3e-137">Response</span></span>

<span data-ttu-id="53f3e-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="53f3e-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53f3e-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="53f3e-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="53f3e-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="53f3e-141">Request</span></span>

<span data-ttu-id="53f3e-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="53f3e-142">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_identitysecuritydefaultsenforcementpolicy"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/identitySecurityDefaultsEnforcementPolicy
Content-type: application/json

{
  "isEnabled": false
}
```

### <a name="response"></a><span data-ttu-id="53f3e-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="53f3e-143">Response</span></span>

<span data-ttu-id="53f3e-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="53f3e-144">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitySecurityDefaultsEnforcementPolicy"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update identitysecuritydefaultsenforcementpolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
