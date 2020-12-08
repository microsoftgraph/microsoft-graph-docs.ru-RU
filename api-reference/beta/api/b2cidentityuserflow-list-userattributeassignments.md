---
title: Список Усераттрибутеассигнментс
description: Получение ресурсов Идентитюсерфловаттрибутеассигнмент из свойства навигации Усераттрибутеассигнментс в b2cIdentityUserFlow.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5a509725149545e43e0fe87026dc9a3b3fd4f05e
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581350"
---
# <a name="list-userattributeassignments"></a><span data-ttu-id="d545d-103">Список Усераттрибутеассигнментс</span><span class="sxs-lookup"><span data-stu-id="d545d-103">List userAttributeAssignments</span></span>

<span data-ttu-id="d545d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d545d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d545d-105">Получение ресурсов Идентитюсерфловаттрибутеассигнмент из свойства навигации Усераттрибутеассигнментс в [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span><span class="sxs-lookup"><span data-stu-id="d545d-105">Get the identityUserFlowAttributeAssignment resources from the userAttributeAssignments navigation property in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d545d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d545d-106">Permissions</span></span>

<span data-ttu-id="d545d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d545d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d545d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d545d-109">Permission type</span></span>|<span data-ttu-id="d545d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d545d-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d545d-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d545d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d545d-112">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d545d-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d545d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d545d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d545d-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="d545d-114">Not supported</span></span>|
|<span data-ttu-id="d545d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d545d-115">Application</span></span>|<span data-ttu-id="d545d-116">Идентитюсерфлов. Read. ALL, Идентитюсерфлов. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="d545d-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d545d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d545d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d545d-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d545d-118">Optional query parameters</span></span>

<span data-ttu-id="d545d-119">Этот метод поддерживает `$select` Параметры и `$expand` для получения сведений об атрибуте пользовательского процесса.</span><span class="sxs-lookup"><span data-stu-id="d545d-119">This method supports the `$select` and `$expand` parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="d545d-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d545d-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d545d-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d545d-121">Request headers</span></span>

|<span data-ttu-id="d545d-122">Имя</span><span class="sxs-lookup"><span data-stu-id="d545d-122">Name</span></span>|<span data-ttu-id="d545d-123">Описание</span><span class="sxs-lookup"><span data-stu-id="d545d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d545d-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d545d-124">Authorization</span></span>|<span data-ttu-id="d545d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d545d-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d545d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d545d-127">Request body</span></span>

<span data-ttu-id="d545d-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d545d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d545d-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="d545d-129">Response</span></span>

<span data-ttu-id="d545d-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [идентитюсерфловаттрибутеассигнмент](../resources/identityuserflowattributeassignment.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d545d-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d545d-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="d545d-131">Examples</span></span>

### <a name="example-1-list-userattributeassignments-in-a-b2cidentityuserflow"></a><span data-ttu-id="d545d-132">Пример 1: List Усераттрибутеассигнментс in a b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="d545d-132">Example 1: List userAttributeAssignments in a b2cIdentityUserFlow</span></span>

#### <a name="request"></a><span data-ttu-id="d545d-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d545d-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?
```

#### <a name="response"></a><span data-ttu-id="d545d-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="d545d-134">Response</span></span>

<span data-ttu-id="d545d-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d545d-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ]
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": []
        }
    ]
}
```

### <a name="example-2-list-userattributeassignments-in-a-b2cidentityuserflow-and-expand-userattribute"></a><span data-ttu-id="d545d-136">Пример 2: List Усераттрибутеассигнментс in a b2cIdentityUserFlow и Expand Усераттрибуте</span><span class="sxs-lookup"><span data-stu-id="d545d-136">Example 2: List userAttributeAssignments in a b2cIdentityUserFlow and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="d545d-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="d545d-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?$expand=userAttribute
```

#### <a name="response"></a><span data-ttu-id="d545d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="d545d-138">Response</span></span>

<span data-ttu-id="d545d-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d545d-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.BuiltInUserFlowAttribute",
                "id": "City",
                "displayName": "City",
                "description": "your city",
                "userFlowAttributeType": "builtIn",
                "dataType": "string"
            }
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": [],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.CustomUserFlowAttribute",
                "id": "extension_guid_shoeSize",
                "displayName": "Shoe size",
                "description": "Your shoe size",
                "userFlowAttributeType": "custom",
                "dataType": "string"
            }
        }
    ]
}
```
