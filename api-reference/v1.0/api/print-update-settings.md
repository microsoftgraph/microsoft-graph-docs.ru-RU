---
title: Обновление printSettings
description: Обновление параметров для клиента для службы универсальной печати.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: cc1af332871ef5d527bff235ef25906c4a739540
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517505"
---
# <a name="update-printsettings"></a><span data-ttu-id="61afb-103">Обновление printSettings</span><span class="sxs-lookup"><span data-stu-id="61afb-103">Update printSettings</span></span>
<span data-ttu-id="61afb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61afb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="61afb-105">Обновление параметров для клиента для службы универсальной печати.</span><span class="sxs-lookup"><span data-stu-id="61afb-105">Update tenant-wide settings for the Universal Print service.</span></span>

## <a name="permissions"></a><span data-ttu-id="61afb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="61afb-106">Permissions</span></span>
<span data-ttu-id="61afb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61afb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="61afb-109">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="61afb-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="61afb-110">Подписанный пользователем должен быть [администратором принтера.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)</span><span class="sxs-lookup"><span data-stu-id="61afb-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="61afb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="61afb-111">Permission type</span></span> | <span data-ttu-id="61afb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="61afb-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="61afb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="61afb-113">Delegated (work or school account)</span></span>| <span data-ttu-id="61afb-114">PrintSettings.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61afb-114">PrintSettings.ReadWrite.All</span></span> |
|<span data-ttu-id="61afb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="61afb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61afb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61afb-116">Not Supported.</span></span>|
|<span data-ttu-id="61afb-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="61afb-117">Application</span></span>|<span data-ttu-id="61afb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61afb-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="61afb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="61afb-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/settings
```

## <a name="request-headers"></a><span data-ttu-id="61afb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="61afb-120">Request headers</span></span>
|<span data-ttu-id="61afb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="61afb-121">Name</span></span>|<span data-ttu-id="61afb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="61afb-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="61afb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="61afb-123">Authorization</span></span>|<span data-ttu-id="61afb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61afb-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="61afb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="61afb-126">Content-Type</span></span>|<span data-ttu-id="61afb-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="61afb-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="61afb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="61afb-129">Request body</span></span>
<span data-ttu-id="61afb-130">В теле запроса укажи значения для соответствующих полей [printSettings,](../resources/printsettings.md) которые должны быть обновлены.</span><span class="sxs-lookup"><span data-stu-id="61afb-130">In the request body, supply the values for the relevant [printSettings](../resources/printsettings.md) fields that should be updated.</span></span> <span data-ttu-id="61afb-131">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="61afb-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="61afb-132">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="61afb-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="61afb-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="61afb-133">Property</span></span>     | <span data-ttu-id="61afb-134">Тип</span><span class="sxs-lookup"><span data-stu-id="61afb-134">Type</span></span>        | <span data-ttu-id="61afb-135">Описание</span><span class="sxs-lookup"><span data-stu-id="61afb-135">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="61afb-136">documentConversionEnabled</span><span class="sxs-lookup"><span data-stu-id="61afb-136">documentConversionEnabled</span></span>|<span data-ttu-id="61afb-137">Логический</span><span class="sxs-lookup"><span data-stu-id="61afb-137">Boolean</span></span>|<span data-ttu-id="61afb-138">Указывает, включено ли преобразование документов для клиента.</span><span class="sxs-lookup"><span data-stu-id="61afb-138">Specifies whether document conversion is enabled for the tenant.</span></span> <span data-ttu-id="61afb-139">Если преобразование документов включено, служба универсальной печати автоматически преобразует документы в формат, совместимый с принтером (например, XPS в PDF) при необходимости.</span><span class="sxs-lookup"><span data-stu-id="61afb-139">If document conversion is enabled, Universal Print service will automatically convert documents into a format compatible with the printer (for example, XPS to PDF) when needed.</span></span>|

## <a name="response"></a><span data-ttu-id="61afb-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="61afb-140">Response</span></span>

<span data-ttu-id="61afb-141">При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.</span><span class="sxs-lookup"><span data-stu-id="61afb-141">If successful, this method returns a `204 No Content` response code and an empty response body.</span></span>

## <a name="examples"></a><span data-ttu-id="61afb-142">Примеры</span><span class="sxs-lookup"><span data-stu-id="61afb-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="61afb-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="61afb-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/settings
Content-type: application/json

{
  "documentConversionEnabled": true
}
```

### <a name="response"></a><span data-ttu-id="61afb-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="61afb-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printSettings"
}
-->
``` http
HTTP/1.1 204 No Content
```

