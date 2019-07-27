---
title: Удаление участника
description: Используйте этот API для удаления члена (пользователя или группы) из административной единицы.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c307a802e2d574950b89c3f5644b5fbf70d90e34
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917935"
---
# <a name="remove-a-member"></a><span data-ttu-id="8c019-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="8c019-103">Remove a member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c019-104">Используйте этот API для удаления члена (пользователя или группы) из административной единицы.</span><span class="sxs-lookup"><span data-stu-id="8c019-104">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="8c019-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c019-105">Permissions</span></span>
<span data-ttu-id="8c019-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c019-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8c019-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c019-108">Permission type</span></span>      | <span data-ttu-id="8c019-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c019-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c019-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c019-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c019-111">AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="8c019-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8c019-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c019-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c019-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c019-113">Not supported.</span></span>    |
|<span data-ttu-id="8c019-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c019-114">Application</span></span> | <span data-ttu-id="8c019-115">AdministrativeUnit. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="8c019-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c019-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c019-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="8c019-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c019-117">Request headers</span></span>
| <span data-ttu-id="8c019-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8c019-118">Name</span></span>      |<span data-ttu-id="8c019-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8c019-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8c019-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c019-120">Authorization</span></span>  | <span data-ttu-id="8c019-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c019-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c019-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8c019-123">Request body</span></span>
<span data-ttu-id="8c019-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8c019-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c019-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c019-125">Response</span></span>

<span data-ttu-id="8c019-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="8c019-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c019-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8c019-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c019-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c019-129">Request</span></span>
<span data-ttu-id="8c019-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c019-130">Here is an example of the request.</span></span> <span data-ttu-id="8c019-131">В приведенном ниже примере id1 представляет идентификатор целевого административного подразделения, а id2 представляет уникальный идентификатор удаляемого пользователя или группы из административного модуля адресного.</span><span class="sxs-lookup"><span data-stu-id="8c019-131">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="8c019-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c019-132">Response</span></span>
<span data-ttu-id="8c019-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8c019-133">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
