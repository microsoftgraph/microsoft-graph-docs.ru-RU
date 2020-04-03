---
title: Удаление участника
description: Используйте этот API для удаления члена (пользователя или группы) из административной единицы.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3774df54f73c7e08456b3412a65378cfb51cefcf
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123344"
---
# <a name="remove-a-member"></a><span data-ttu-id="00658-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="00658-103">Remove a member</span></span>

<span data-ttu-id="00658-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00658-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00658-105">Используйте этот API для удаления члена (пользователя или группы) из административной единицы.</span><span class="sxs-lookup"><span data-stu-id="00658-105">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="00658-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00658-106">Permissions</span></span>
<span data-ttu-id="00658-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00658-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="00658-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00658-109">Permission type</span></span>      | <span data-ttu-id="00658-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00658-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00658-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00658-111">Delegated (work or school account)</span></span> | <span data-ttu-id="00658-112">AdministrativeUnit. ReadWrite. ALL, Directory. AccessAsUser. ALL</span><span class="sxs-lookup"><span data-stu-id="00658-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="00658-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00658-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00658-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00658-114">Not supported.</span></span>    |
|<span data-ttu-id="00658-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00658-115">Application</span></span> | <span data-ttu-id="00658-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00658-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00658-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00658-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="00658-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00658-118">Request headers</span></span>
| <span data-ttu-id="00658-119">Имя</span><span class="sxs-lookup"><span data-stu-id="00658-119">Name</span></span>      |<span data-ttu-id="00658-120">Описание</span><span class="sxs-lookup"><span data-stu-id="00658-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="00658-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="00658-121">Authorization</span></span>  | <span data-ttu-id="00658-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="00658-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="00658-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00658-124">Request body</span></span>
<span data-ttu-id="00658-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="00658-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00658-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="00658-126">Response</span></span>

<span data-ttu-id="00658-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="00658-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00658-129">Пример</span><span class="sxs-lookup"><span data-stu-id="00658-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00658-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="00658-130">Request</span></span>
<span data-ttu-id="00658-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00658-131">Here is an example of the request.</span></span> <span data-ttu-id="00658-132">В приведенном ниже примере id1 представляет идентификатор целевого административного подразделения, а id2 представляет уникальный идентификатор удаляемого пользователя или группы из административного модуля адресного.</span><span class="sxs-lookup"><span data-stu-id="00658-132">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="00658-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="00658-133">Response</span></span>
<span data-ttu-id="00658-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00658-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
