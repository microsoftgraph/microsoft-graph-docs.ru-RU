---
title: Get printSettings
description: Извлечение параметров для всей клиентской службы печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f7899af4ea72307a4f9c725d131601d30cf90317
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517985"
---
# <a name="get-printsettings"></a><span data-ttu-id="47c86-103">Get printSettings</span><span class="sxs-lookup"><span data-stu-id="47c86-103">Get printSettings</span></span>

<span data-ttu-id="47c86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47c86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="47c86-105">Извлечение параметров для всей клиентской службы печати.</span><span class="sxs-lookup"><span data-stu-id="47c86-105">Retrieve tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="47c86-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47c86-106">Permissions</span></span>
<span data-ttu-id="47c86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47c86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="47c86-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="47c86-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="47c86-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="47c86-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="47c86-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47c86-111">Permission type</span></span> | <span data-ttu-id="47c86-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47c86-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="47c86-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47c86-113">Delegated (work or school account)</span></span>| <span data-ttu-id="47c86-114">PrintSettings.Read.All, PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47c86-114">PrintSettings.Read.All, PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="47c86-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47c86-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47c86-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47c86-116">Not Supported.</span></span>|
|<span data-ttu-id="47c86-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="47c86-117">Application</span></span>|<span data-ttu-id="47c86-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47c86-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="47c86-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47c86-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/settings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="47c86-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="47c86-120">Optional query parameters</span></span>
<span data-ttu-id="47c86-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="47c86-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="47c86-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="47c86-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="47c86-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47c86-123">Request headers</span></span>
| <span data-ttu-id="47c86-124">Имя</span><span class="sxs-lookup"><span data-stu-id="47c86-124">Name</span></span>      |<span data-ttu-id="47c86-125">Описание</span><span class="sxs-lookup"><span data-stu-id="47c86-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47c86-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47c86-126">Authorization</span></span> | <span data-ttu-id="47c86-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47c86-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47c86-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47c86-129">Request body</span></span>
<span data-ttu-id="47c86-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47c86-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47c86-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="47c86-131">Response</span></span>
<span data-ttu-id="47c86-132">В случае успешной работы этот метод возвращает код отклика и объект `200 OK` [printSettings](../resources/printsettings.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="47c86-132">If successful, this method returns a `200 OK` response code and a [printSettings](../resources/printsettings.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="47c86-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="47c86-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="47c86-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="47c86-134">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_printsettings"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/settings
```


### <a name="response"></a><span data-ttu-id="47c86-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="47c86-135">Response</span></span>
<span data-ttu-id="47c86-136">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="47c86-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/settings",
  "documentConversionEnabled": true
}
```

