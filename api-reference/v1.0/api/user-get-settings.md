---
title: Получение параметров
description: Чтение объекта settings пользователя и организации.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 59685923c939dae2ae066a2e146398ea8f87a05c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567937"
---
# <a name="get-settings"></a><span data-ttu-id="ea34a-103">Получение параметров</span><span class="sxs-lookup"><span data-stu-id="ea34a-103">Get settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea34a-104">Чтение объекта [settings](../resources/user-settings.md) пользователя и организации.</span><span class="sxs-lookup"><span data-stu-id="ea34a-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="ea34a-105">Сведения об обновлении свойства объекта [settings](../resources/user-settings.md) см. в статье [Обновление параметров пользователя](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="ea34a-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea34a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea34a-106">Permissions</span></span>

<span data-ttu-id="ea34a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea34a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea34a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea34a-109">Permission type</span></span>      | <span data-ttu-id="ea34a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ea34a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea34a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea34a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea34a-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea34a-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea34a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea34a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea34a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea34a-114">Not supported.</span></span>    |
|<span data-ttu-id="ea34a-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="ea34a-115">Application</span></span> | <span data-ttu-id="ea34a-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea34a-116">User.Read.All, User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea34a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea34a-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="ea34a-118">Запрос с параметрами user id или userPrincipalName доступен только пользователю или пользователю с разрешениями User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="ea34a-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="ea34a-119">Дополнительные сведения см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea34a-119">To learn more, please see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="ea34a-120">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea34a-120">Request body</span></span>

<span data-ttu-id="ea34a-121">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ea34a-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea34a-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea34a-122">Response</span></span>

<span data-ttu-id="ea34a-123">При успешном выполнении этот метод возвращает код отклика `200 OK` и объект [user settings](../resources/user-settings.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ea34a-123">If successful, this method returns a `200 OK` response code and [user](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea34a-124">Пример</span><span class="sxs-lookup"><span data-stu-id="ea34a-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ea34a-125">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea34a-125">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="ea34a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="ea34a-126">Response</span></span>

<span data-ttu-id="ea34a-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea34a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
