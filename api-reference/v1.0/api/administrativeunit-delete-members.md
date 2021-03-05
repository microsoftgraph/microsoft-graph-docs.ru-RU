---
title: Удаление участника
description: Используйте этот API для удаления участника (пользователя или группы) из административного подразделения.
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: c0af2db5358505e3510ad4cc6eaefa96bc431842
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442525"
---
# <a name="remove-a-member"></a><span data-ttu-id="9dcdc-103">Удаление участника</span><span class="sxs-lookup"><span data-stu-id="9dcdc-103">Remove a member</span></span>

<span data-ttu-id="9dcdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9dcdc-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9dcdc-105">Используйте этот API для удаления участника (пользователя или группы) из административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="9dcdc-105">Use this API to remove a member (user or group) from an administrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="9dcdc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9dcdc-106">Permissions</span></span>
<span data-ttu-id="9dcdc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9dcdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9dcdc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9dcdc-109">Permission type</span></span>      | <span data-ttu-id="9dcdc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9dcdc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9dcdc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9dcdc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9dcdc-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9dcdc-112">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9dcdc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9dcdc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9dcdc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9dcdc-114">Not supported.</span></span>    |
|<span data-ttu-id="9dcdc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9dcdc-115">Application</span></span> | <span data-ttu-id="9dcdc-116">AdministrativeUnit.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9dcdc-116">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9dcdc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9dcdc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /directory/administrativeUnits/{id}/members/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9dcdc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9dcdc-118">Request headers</span></span>
| <span data-ttu-id="9dcdc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9dcdc-119">Name</span></span>      |<span data-ttu-id="9dcdc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9dcdc-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9dcdc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9dcdc-121">Authorization</span></span>  | <span data-ttu-id="9dcdc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9dcdc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9dcdc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9dcdc-124">Request body</span></span>
<span data-ttu-id="9dcdc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9dcdc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9dcdc-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dcdc-126">Response</span></span>

<span data-ttu-id="9dcdc-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9dcdc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9dcdc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9dcdc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9dcdc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9dcdc-130">Request</span></span>
<span data-ttu-id="9dcdc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9dcdc-131">Here is an example of the request.</span></span> <span data-ttu-id="9dcdc-132">В приведенной ниже примере идентификатор id1 представляет идентификатор целевого административного подразделения, а id2 — уникальный идентификатор пользователя или группы членов, которые будут удалены из целевого административного подразделения.</span><span class="sxs-lookup"><span data-stu-id="9dcdc-132">In the example below, id1 represents the identifier for the target administrative unit, and id2 represents the unique identifier for the member user or group to be removed from the targetted administrative unit.</span></span> 

```http
DELETE https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id1}/members/{id2}/$ref
```

##### <a name="response"></a><span data-ttu-id="9dcdc-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9dcdc-133">Response</span></span>
<span data-ttu-id="9dcdc-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9dcdc-134">Here is an example of the response.</span></span>
 
```http
HTTP/1.1 204 No Content
```
