---
title: Создание Усерсаурце
description: Создание нового объекта Усерсаурце.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: 9ff054926611c990f8db0a2f868ac3449708436f
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597739"
---
# <a name="create-usersource"></a><span data-ttu-id="deb4d-103">Создание Усерсаурце</span><span class="sxs-lookup"><span data-stu-id="deb4d-103">Create userSource</span></span>

<span data-ttu-id="deb4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deb4d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deb4d-105">Создание нового объекта [усерсаурце](../resources/usersource.md) .</span><span class="sxs-lookup"><span data-stu-id="deb4d-105">Create a new [userSource](../resources/usersource.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="deb4d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="deb4d-106">Permissions</span></span>

<span data-ttu-id="deb4d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="deb4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="deb4d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="deb4d-109">Permission type</span></span>|<span data-ttu-id="deb4d-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="deb4d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="deb4d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="deb4d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="deb4d-112">User.Read</span><span class="sxs-lookup"><span data-stu-id="deb4d-112">User.Read</span></span>|
|<span data-ttu-id="deb4d-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="deb4d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="deb4d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deb4d-114">Not supported.</span></span>|
|<span data-ttu-id="deb4d-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="deb4d-115">Application</span></span>|<span data-ttu-id="deb4d-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="deb4d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="deb4d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="deb4d-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{ediscoveryCaseId}/custodians/{custodianId}/userSources
```

## <a name="request-headers"></a><span data-ttu-id="deb4d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="deb4d-118">Request headers</span></span>

|<span data-ttu-id="deb4d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="deb4d-119">Name</span></span>|<span data-ttu-id="deb4d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="deb4d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="deb4d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="deb4d-121">Authorization</span></span>|<span data-ttu-id="deb4d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb4d-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="deb4d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="deb4d-124">Content-Type</span></span>|<span data-ttu-id="deb4d-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="deb4d-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="deb4d-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="deb4d-127">Request body</span></span>

<span data-ttu-id="deb4d-128">В тексте запроса добавьте представление объекта [усерсаурце](../resources/usersource.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="deb4d-128">In the request body, supply a JSON representation of the [userSource](../resources/usersource.md) object.</span></span>

<span data-ttu-id="deb4d-129">В следующей таблице приведены свойства, необходимые при создании [усерсаурце](../resources/usersource.md).</span><span class="sxs-lookup"><span data-stu-id="deb4d-129">The following table shows the properties that are required when you create the [userSource](../resources/usersource.md).</span></span>

|<span data-ttu-id="deb4d-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="deb4d-130">Property</span></span>|<span data-ttu-id="deb4d-131">Тип</span><span class="sxs-lookup"><span data-stu-id="deb4d-131">Type</span></span>|<span data-ttu-id="deb4d-132">Описание</span><span class="sxs-lookup"><span data-stu-id="deb4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deb4d-133">email</span><span class="sxs-lookup"><span data-stu-id="deb4d-133">email</span></span>|<span data-ttu-id="deb4d-134">String</span><span class="sxs-lookup"><span data-stu-id="deb4d-134">String</span></span>|<span data-ttu-id="deb4d-135">SMTP-адрес пользователя.</span><span class="sxs-lookup"><span data-stu-id="deb4d-135">SMTP address of the user.</span></span>|
|<span data-ttu-id="deb4d-136">инклудедсаурцес</span><span class="sxs-lookup"><span data-stu-id="deb4d-136">includedSources</span></span>|<span data-ttu-id="deb4d-137">sourceType</span><span class="sxs-lookup"><span data-stu-id="deb4d-137">sourceType</span></span>|<span data-ttu-id="deb4d-138">Указывает, какие источники включены в эту группу.</span><span class="sxs-lookup"><span data-stu-id="deb4d-138">Specifies which sources are included in this group.</span></span> <span data-ttu-id="deb4d-139">Возможные значения: `mailbox`, `site`.</span><span class="sxs-lookup"><span data-stu-id="deb4d-139">Possible values are: `mailbox`, `site`.</span></span>|

## <a name="response"></a><span data-ttu-id="deb4d-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb4d-140">Response</span></span>

<span data-ttu-id="deb4d-141">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [усерсаурце](../resources/usersource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="deb4d-141">If successful, this method returns a `201 Created` response code and a [userSource](../resources/usersource.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="deb4d-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="deb4d-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="deb4d-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="deb4d-143">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_usersource_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/4c8f8f70-7785-4bd4-b296-c98376a2c5e1/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources
Content-Type: application/json
Content-length: 233

{
    "email":"megan@contoso.com",
    "includedSources":"mailbox, site"
}
```

### <a name="response"></a><span data-ttu-id="deb4d-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="deb4d-144">Response</span></span>

<span data-ttu-id="deb4d-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="deb4d-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('4c8f8f70-7785-4bd4-b296-c98376a2c5e1')/custodians('45454331323337443946343043464239')/userSources/$entity",
    "displayName": "Megan Bowen",
    "createdDateTime": "2020-11-06T16:09:08.4905571Z",
    "id": "34383036-3741-4545-3242-373530353435",
    "email": "megan@contoso.com",
    "includedSources": "mailbox,site",
    "createdBy": {
        "user": {
            "id": "c1db6f13-332a-4d84-b111-914383ff9fc9",
            "displayName": null
        }
    }
}
```
