---
title: 'Виртуалендпоинт: getEffectivePermissions'
description: '**GetEffectivePermissions — это функция, которая ретривес действующие разрешения пользователя, прошедшего проверку подлинности, что позволяет скрыть или отключить контент, к которому у текущего пользователя нет доступа.**'
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: 78b58c5ea00e1b170d831a91f5dc3ff1569bd0d7
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378626"
---
# <a name="virtualendpoint-geteffectivepermissions"></a><span data-ttu-id="0ddbc-103">Виртуалендпоинт: getEffectivePermissions</span><span class="sxs-lookup"><span data-stu-id="0ddbc-103">virtualEndpoint: getEffectivePermissions</span></span>

<span data-ttu-id="0ddbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ddbc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0ddbc-105">Просмотр действующих разрешений текущего пользователя, прошедшего проверку подлинности.</span><span class="sxs-lookup"><span data-stu-id="0ddbc-105">View the effective permissions of the currently authenticated user.</span></span> <span data-ttu-id="0ddbc-106">GetEffectivePermissions — это функция, которая ретривес действующие разрешения пользователя, прошедшего проверку подлинности, что позволяет скрыть или отключить контент, к которому у текущего пользователя нет доступа.</span><span class="sxs-lookup"><span data-stu-id="0ddbc-106">GetEffectivePermissions is a function that retrives the effective permissions of the currently authenticated user, which helps UX hide or disable content that the current user doesn't have access to.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ddbc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ddbc-107">Permissions</span></span>

<span data-ttu-id="0ddbc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ddbc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ddbc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ddbc-110">Permission type</span></span>|<span data-ttu-id="0ddbc-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ddbc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ddbc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ddbc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ddbc-113">Клаудпк. ReadWrite. ALL, Клаудпк. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="0ddbc-113">CloudPC.ReadWrite.All, CloudPC.Read.All</span></span>|
|<span data-ttu-id="0ddbc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ddbc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ddbc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ddbc-115">Not supported.</span></span>|
|<span data-ttu-id="0ddbc-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ddbc-116">Application</span></span>| <span data-ttu-id="0ddbc-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ddbc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ddbc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ddbc-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="0ddbc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ddbc-119">Request headers</span></span>

| <span data-ttu-id="0ddbc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0ddbc-120">Name</span></span>          | <span data-ttu-id="0ddbc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0ddbc-121">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0ddbc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ddbc-122">Authorization</span></span> | <span data-ttu-id="0ddbc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ddbc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ddbc-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ddbc-125">Request body</span></span>

<span data-ttu-id="0ddbc-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ddbc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ddbc-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ddbc-127">Response</span></span>

<span data-ttu-id="0ddbc-128">При успешном выполнении эта функция возвращает код отклика `200 OK` и коллекцию String в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="0ddbc-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span> <span data-ttu-id="0ddbc-129">Если у пользователя есть полные разрешения, ответ — `["*"]` .</span><span class="sxs-lookup"><span data-stu-id="0ddbc-129">If the user has full permissions, the response is `["*"]`.</span></span>

## <a name="examples"></a><span data-ttu-id="0ddbc-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="0ddbc-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0ddbc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ddbc-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "virtualendpoint_geteffectivepermissions"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/getEffectivePermissions
```

### <a name="response"></a><span data-ttu-id="0ddbc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ddbc-132">Response</span></span>

<span data-ttu-id="0ddbc-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0ddbc-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK

Content-Type: application/json
{
  "value": [
    "Microsoft.CloudPC/CloudPCs/Read"
  ]
}
```
