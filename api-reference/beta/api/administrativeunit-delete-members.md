---
title: Удаление члена
description: Используйте этот интерфейс API для удаления участника (пользователя или группы) из административного подразделения.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 29ea8aa11850909c9e7122c55dc6c686ae9135a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528083"
---
# <a name="remove-a-member"></a><span data-ttu-id="90707-103">Удаление члена</span><span class="sxs-lookup"><span data-stu-id="90707-103">Remove a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90707-104">Используйте этот интерфейс API для удаления участника (пользователя или группы) из административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="90707-104">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="90707-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90707-105">Permissions</span></span>
<span data-ttu-id="90707-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90707-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="90707-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90707-108">Permission type</span></span>      | <span data-ttu-id="90707-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90707-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90707-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90707-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90707-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="90707-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="90707-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90707-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90707-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90707-113">Not supported.</span></span>    |
|<span data-ttu-id="90707-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90707-114">Application</span></span> | <span data-ttu-id="90707-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90707-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90707-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90707-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="90707-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90707-117">Request headers</span></span>
| <span data-ttu-id="90707-118">Имя</span><span class="sxs-lookup"><span data-stu-id="90707-118">Name</span></span>      |<span data-ttu-id="90707-119">Описание</span><span class="sxs-lookup"><span data-stu-id="90707-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="90707-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90707-120">Authorization</span></span>  | <span data-ttu-id="90707-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90707-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90707-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90707-123">Request body</span></span>
<span data-ttu-id="90707-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90707-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90707-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="90707-125">Response</span></span>

<span data-ttu-id="90707-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="90707-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90707-128">Пример</span><span class="sxs-lookup"><span data-stu-id="90707-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90707-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="90707-129">Request</span></span>
<span data-ttu-id="90707-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90707-130">Here is an example of the request.</span></span> <span data-ttu-id="90707-131">В приведенном ниже примере id1 представляет идентификатор для конечного единица и id2 представляет уникальный идентификатор участника пользователя или группы для удаления из targetted единица.</span><span class="sxs-lookup"><span data-stu-id="90707-131">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="90707-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="90707-132">Response</span></span>
<span data-ttu-id="90707-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90707-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-delete-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
