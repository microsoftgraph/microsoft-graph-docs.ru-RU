---
title: Получение параметров
description: Чтение объекта settings пользователя и организации.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 82d6897f0637090db704a5ca174f75f04446ba13
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844171"
---
# <a name="get-settings"></a><span data-ttu-id="a96ce-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="a96ce-103">Get settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a96ce-104">Чтение объекта User и Organization [усерсеттингс](../resources/usersettings.md) .</span><span class="sxs-lookup"><span data-stu-id="a96ce-104">Read the user and organization [userSettings](../resources/usersettings.md) object.</span></span>
<span data-ttu-id="a96ce-105">Чтобы узнать, как обновить свойства объекта [усерсеттингс](../resources/usersettings.md) , ознакомьтесь со статьей [Обновление параметров пользователя](usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="a96ce-105">To learn how to update the properties of the [userSettings](../resources/usersettings.md) object, see [update user settings](usersettings-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a96ce-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a96ce-106">Permissions</span></span>

<span data-ttu-id="a96ce-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a96ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a96ce-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a96ce-109">Permission type</span></span>      | <span data-ttu-id="a96ce-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a96ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a96ce-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a96ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a96ce-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a96ce-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="a96ce-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a96ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a96ce-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a96ce-114">Not supported.</span></span>    |
|<span data-ttu-id="a96ce-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="a96ce-115">Application</span></span> | <span data-ttu-id="a96ce-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a96ce-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a96ce-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a96ce-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="a96ce-118">Запрос с параметрами user id или userPrincipalName доступен только пользователю или пользователю с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="a96ce-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="a96ce-119">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a96ce-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="a96ce-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a96ce-120">Request body</span></span>

<span data-ttu-id="a96ce-121">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a96ce-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a96ce-122">Ответ</span><span class="sxs-lookup"><span data-stu-id="a96ce-122">Response</span></span>

<span data-ttu-id="a96ce-123">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [усерсеттингс](../resources/usersettings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a96ce-123">If successful, this method returns a `200 OK` response code and [userSettings](../resources/usersettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a96ce-124">Пример</span><span class="sxs-lookup"><span data-stu-id="a96ce-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a96ce-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="a96ce-125">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="a96ce-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="a96ce-126">Response</span></span>

<span data-ttu-id="a96ce-p104">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a96ce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
