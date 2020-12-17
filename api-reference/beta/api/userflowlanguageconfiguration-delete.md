---
title: Удаление userFlowLanguageConfiguration
description: Удаляет объект userFlowLanguageConfiguration из пользовательского потока B2C.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9f9396e9522e4f2f6df536e687526b261ce78e6b
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706490"
---
# <a name="delete-userflowlanguageconfiguration"></a><span data-ttu-id="7cd37-103">Удаление userFlowLanguageConfiguration</span><span class="sxs-lookup"><span data-stu-id="7cd37-103">Delete userFlowLanguageConfiguration</span></span>

<span data-ttu-id="7cd37-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cd37-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7cd37-105">Удаляет объект [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) из пользовательского потока [B2C Azure AD.](../resources/b2cidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="7cd37-105">Deletes a [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) object from a [Azure AD B2C user flow](../resources/b2cidentityuserflow.md).</span></span>

<span data-ttu-id="7cd37-106">**Примечание.** Вы не можете удалить языки из пользовательского [потока Azure Active Directory.](../resources/b2xidentityuserflow.md)</span><span class="sxs-lookup"><span data-stu-id="7cd37-106">**Note:** You cannot delete languages from an [Azure Active Directory user flow](../resources/b2xidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7cd37-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7cd37-107">Permissions</span></span>

<span data-ttu-id="7cd37-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cd37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cd37-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7cd37-110">Permission type</span></span>      | <span data-ttu-id="7cd37-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7cd37-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cd37-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7cd37-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7cd37-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cd37-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="7cd37-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7cd37-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="7cd37-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7cd37-115">Not supported.</span></span>|
|<span data-ttu-id="7cd37-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="7cd37-116">Application</span></span>|<span data-ttu-id="7cd37-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cd37-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="7cd37-118">Учетная запись для работы или учебного заведения должна принадлежать одной из следующих ролей:</span><span class="sxs-lookup"><span data-stu-id="7cd37-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="7cd37-119">Глобальный администратор</span><span class="sxs-lookup"><span data-stu-id="7cd37-119">Global administrator</span></span>
* <span data-ttu-id="7cd37-120">Администратор потока пользователей внешнего удостоверения</span><span class="sxs-lookup"><span data-stu-id="7cd37-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="7cd37-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7cd37-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/b2cUserFlows/{id}/languages/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7cd37-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7cd37-122">Request headers</span></span>

|<span data-ttu-id="7cd37-123">Имя</span><span class="sxs-lookup"><span data-stu-id="7cd37-123">Name</span></span>|<span data-ttu-id="7cd37-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7cd37-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="7cd37-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7cd37-125">Authorization</span></span>|<span data-ttu-id="7cd37-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7cd37-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cd37-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7cd37-128">Request body</span></span>

<span data-ttu-id="7cd37-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7cd37-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cd37-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cd37-130">Response</span></span>

<span data-ttu-id="7cd37-131">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="7cd37-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7cd37-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="7cd37-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7cd37-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7cd37-133">Request</span></span>

<span data-ttu-id="7cd37-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7cd37-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_userflowlanguageconfiguration"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/es-ES
```

### <a name="response"></a><span data-ttu-id="7cd37-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="7cd37-135">Response</span></span>

<span data-ttu-id="7cd37-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7cd37-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
