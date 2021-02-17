---
title: Get temporaryAccessPassAuthenticationMethod
description: Чтение свойств и связей временного объектаAccessPassAuthenticationMethod.
author: inbarckMS
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 154afeae29769fb29122f6f35503b919bfad0e7e
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272662"
---
# <a name="get-temporaryaccesspassauthenticationmethod"></a><span data-ttu-id="de5fe-103">Get temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="de5fe-103">Get temporaryAccessPassAuthenticationMethod</span></span>
<span data-ttu-id="de5fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de5fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de5fe-105">Извлечение отдельного объекта  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="de5fe-105">Retrieve a user's single  [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="de5fe-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="de5fe-106">Permissions</span></span>
<span data-ttu-id="de5fe-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="de5fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-acting-on-self"></a><span data-ttu-id="de5fe-109">Разрешения, действующие на себя</span><span class="sxs-lookup"><span data-stu-id="de5fe-109">Permissions acting on self</span></span>

|<span data-ttu-id="de5fe-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de5fe-110">Permission type</span></span>      | <span data-ttu-id="de5fe-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de5fe-111">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|
| <span data-ttu-id="de5fe-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de5fe-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="de5fe-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="de5fe-113">UserAuthenticationMethod.Read, UserAuthenticationMethod.ReadWrite</span></span> |
| <span data-ttu-id="de5fe-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de5fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de5fe-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de5fe-115">Not supported.</span></span> |
| <span data-ttu-id="de5fe-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de5fe-116">Application</span></span>                            | <span data-ttu-id="de5fe-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de5fe-117">Not supported.</span></span> |

### <a name="permissions-acting-on-other-users"></a><span data-ttu-id="de5fe-118">Разрешения, действующие с другими пользователями</span><span class="sxs-lookup"><span data-stu-id="de5fe-118">Permissions acting on other users</span></span>

|<span data-ttu-id="de5fe-119">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="de5fe-119">Permission type</span></span>      | <span data-ttu-id="de5fe-120">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="de5fe-120">Permissions (from least to most privileged)</span></span>              |
|:---------------------------------------|:-------------------------|:-----------------|
| <span data-ttu-id="de5fe-121">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="de5fe-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="de5fe-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de5fe-122">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |
| <span data-ttu-id="de5fe-123">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="de5fe-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de5fe-124">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="de5fe-124">Not supported.</span></span> |
| <span data-ttu-id="de5fe-125">Для приложений</span><span class="sxs-lookup"><span data-stu-id="de5fe-125">Application</span></span>                            | <span data-ttu-id="de5fe-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de5fe-126">UserAuthenticationMethod.Read.All, UserAuthenticationMethod.ReadWrite.All</span></span> |

<span data-ttu-id="de5fe-127">Для делегирования сценариев, в которых администратор действует над другим пользователем, администратору требуется одна [из следующих ролей:](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)</span><span class="sxs-lookup"><span data-stu-id="de5fe-127">For delegated scenarios where an admin is acting on another user, the admin needs [one of the following roles](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles):</span></span>
* <span data-ttu-id="de5fe-128">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="de5fe-128">Global admin</span></span>
* <span data-ttu-id="de5fe-129">Глобальный читатель</span><span class="sxs-lookup"><span data-stu-id="de5fe-129">Global reader</span></span>
* <span data-ttu-id="de5fe-130">Привилегированный администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="de5fe-130">Privileged authentication admin</span></span>
* <span data-ttu-id="de5fe-131">Администратор проверки подлинности</span><span class="sxs-lookup"><span data-stu-id="de5fe-131">Authentication admin</span></span>

## <a name="http-request"></a><span data-ttu-id="de5fe-132">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="de5fe-132">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
GET /users/{id | userPrincipalName}/authentication/temporaryAccessPassMethods/{temporaryAccessPassAuthenticationMethodId}
```


## <a name="request-headers"></a><span data-ttu-id="de5fe-133">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="de5fe-133">Request headers</span></span>
|<span data-ttu-id="de5fe-134">Имя</span><span class="sxs-lookup"><span data-stu-id="de5fe-134">Name</span></span>|<span data-ttu-id="de5fe-135">Описание</span><span class="sxs-lookup"><span data-stu-id="de5fe-135">Description</span></span>|
|:---|:---|
|<span data-ttu-id="de5fe-136">Авторизация</span><span class="sxs-lookup"><span data-stu-id="de5fe-136">Authorization</span></span>|<span data-ttu-id="de5fe-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="de5fe-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="de5fe-139">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="de5fe-139">Request body</span></span>
<span data-ttu-id="de5fe-140">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="de5fe-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="de5fe-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="de5fe-141">Response</span></span>

<span data-ttu-id="de5fe-142">В случае успеха этот метод возвращает код отклика и временный `200 OK` [объектAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="de5fe-142">If successful, this method returns a `200 OK` response code and a [temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de5fe-143">Примеры</span><span class="sxs-lookup"><span data-stu-id="de5fe-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de5fe-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="de5fe-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_temporaryaccesspassauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30
```


### <a name="response"></a><span data-ttu-id="de5fe-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="de5fe-145">Response</span></span>
<span data-ttu-id="de5fe-146">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="de5fe-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
    "id": "30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30",
    "temporaryAccessPass": null,
    "createdDateTime": "String (timestamp)",
    "startDateTime": "String (timestamp)",
    "lifetimeInMinutes": "Integer",
    "isUsableOnce": "Boolean",
    "isUsable": "Boolean",
    "methodUsabilityReason": "String"
  }
}
```
