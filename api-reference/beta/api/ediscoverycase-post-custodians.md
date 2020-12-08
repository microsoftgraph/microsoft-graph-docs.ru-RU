---
title: Создание хранитель
description: Создание нового объекта хранитель.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 7142d00f7fdee7643e5c6c2b755c1c88a1e9f9dc
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597802"
---
# <a name="create-custodian"></a><span data-ttu-id="32363-103">Создание хранитель</span><span class="sxs-lookup"><span data-stu-id="32363-103">Create custodian</span></span>

<span data-ttu-id="32363-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="32363-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32363-105">Создание нового объекта [хранитель](../resources/custodian.md) .</span><span class="sxs-lookup"><span data-stu-id="32363-105">Create a new [custodian](../resources/custodian.md) object.</span></span> <span data-ttu-id="32363-106">После создания объекта хранитель необходимо создать [усерсаурце](../resources/usersource.md) хранитель, чтобы ссылаться на свой почтовый ящик и сайт OneDrive для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="32363-106">After the custodian object is created, you will need to create the custodian's [userSource](../resources/usersource.md) to reference their mailbox and OneDrive for Business site.</span></span>

## <a name="permissions"></a><span data-ttu-id="32363-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32363-107">Permissions</span></span>

<span data-ttu-id="32363-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32363-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32363-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32363-110">Permission type</span></span>|<span data-ttu-id="32363-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="32363-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32363-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32363-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32363-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="32363-113">User.Read</span></span>|
|<span data-ttu-id="32363-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32363-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32363-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32363-115">Not supported.</span></span>|
|<span data-ttu-id="32363-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32363-116">Application</span></span>|<span data-ttu-id="32363-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32363-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32363-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32363-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians
```

## <a name="request-headers"></a><span data-ttu-id="32363-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32363-119">Request headers</span></span>

|<span data-ttu-id="32363-120">Имя</span><span class="sxs-lookup"><span data-stu-id="32363-120">Name</span></span>|<span data-ttu-id="32363-121">Описание</span><span class="sxs-lookup"><span data-stu-id="32363-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="32363-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="32363-122">Authorization</span></span>|<span data-ttu-id="32363-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32363-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="32363-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="32363-125">Content-Type</span></span>|<span data-ttu-id="32363-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="32363-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="32363-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="32363-128">Request body</span></span>

<span data-ttu-id="32363-129">В тексте запроса добавьте представление объекта [хранитель](../resources/custodian.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="32363-129">In the request body, supply a JSON representation of the [custodian](../resources/custodian.md) object.</span></span>

<span data-ttu-id="32363-130">В следующей таблице приведены свойства, необходимые при создании [хранитель](../resources/custodian.md).</span><span class="sxs-lookup"><span data-stu-id="32363-130">The following table shows the properties that are required when you create the [custodian](../resources/custodian.md).</span></span>

|<span data-ttu-id="32363-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="32363-131">Property</span></span>|<span data-ttu-id="32363-132">Тип</span><span class="sxs-lookup"><span data-stu-id="32363-132">Type</span></span>|<span data-ttu-id="32363-133">Описание</span><span class="sxs-lookup"><span data-stu-id="32363-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32363-134">email</span><span class="sxs-lookup"><span data-stu-id="32363-134">email</span></span>|<span data-ttu-id="32363-135">String</span><span class="sxs-lookup"><span data-stu-id="32363-135">String</span></span>|<span data-ttu-id="32363-136">Основной SMTP-адрес хранитель.</span><span class="sxs-lookup"><span data-stu-id="32363-136">Custodian's primary SMTP address.</span></span> <span data-ttu-id="32363-137">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="32363-137">Required.</span></span>|
|<span data-ttu-id="32363-138">апплихолдтосаурцес</span><span class="sxs-lookup"><span data-stu-id="32363-138">applyHoldToSources</span></span>|<span data-ttu-id="32363-139">Логический</span><span class="sxs-lookup"><span data-stu-id="32363-139">Boolean</span></span>|<span data-ttu-id="32363-140">Указывает, применяется ли удержание к источникам хранитель (таким как почтовые ящики, сайты или рабочие группы).</span><span class="sxs-lookup"><span data-stu-id="32363-140">Indicates whether a hold is applied to the custodian's sources (such as mailboxes, sites, or Teams).</span></span>|

## <a name="response"></a><span data-ttu-id="32363-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="32363-141">Response</span></span>

<span data-ttu-id="32363-142">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [хранитель](../resources/custodian.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="32363-142">If successful, this method returns a `201 Created` response code and a [custodian](../resources/custodian.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="32363-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="32363-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="32363-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="32363-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_custodian_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians
Content-Type: application/json
Content-length: 279

{
    "email":"AdeleV@contoso.com",
    "applyHoldToSources":"true"
}
```

### <a name="response"></a><span data-ttu-id="32363-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="32363-145">Response</span></span>

<span data-ttu-id="32363-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="32363-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.custodian"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians/$entity",
    "email": "AdeleV@contoso.com",
    "applyHoldToSources": false,
    "status": "active",
    "createdDateTime": "2020-10-30T20:47:01.7724531Z",
    "lastModifiedDateTime": "2020-10-30T20:47:02.2512381Z",
    "releasedDateTime": null,
    "acknowledgedDateTime": null,
    "id": "45353243323138344430413038363846",
    "displayName": "Adele Vance"
}
```
