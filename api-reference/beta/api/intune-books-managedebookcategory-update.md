---
title: Обновление managedEBookCategory
description: Обновление свойства объекта managedEBookCategory.
author: tfitzmac
ms.openlocfilehash: 5dea4bce1750617367f972f64a734ac151d2676f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333658"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="a179c-103">Обновление managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="a179c-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="a179c-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a179c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a179c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a179c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a179c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a179c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a179c-107">Обновление свойства объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="a179c-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a179c-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="a179c-108">Prerequisites</span></span>
<span data-ttu-id="a179c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a179c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a179c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a179c-111">Permission type</span></span>|<span data-ttu-id="a179c-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="a179c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a179c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a179c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a179c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a179c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a179c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a179c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a179c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a179c-116">Not supported.</span></span>|
|<span data-ttu-id="a179c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a179c-117">Application</span></span>|<span data-ttu-id="a179c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a179c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a179c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a179c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="a179c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a179c-120">Request headers</span></span>
|<span data-ttu-id="a179c-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a179c-121">Header</span></span>|<span data-ttu-id="a179c-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a179c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a179c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a179c-123">Authorization</span></span>|<span data-ttu-id="a179c-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="a179c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a179c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a179c-125">Accept</span></span>|<span data-ttu-id="a179c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a179c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a179c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a179c-127">Request body</span></span>
<span data-ttu-id="a179c-128">В тексте запроса укажите представление JSON для объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="a179c-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="a179c-129">В следующей таблице показаны свойства, которые необходимы для создания [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="a179c-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="a179c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="a179c-130">Property</span></span>|<span data-ttu-id="a179c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="a179c-131">Type</span></span>|<span data-ttu-id="a179c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="a179c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a179c-133">id</span><span class="sxs-lookup"><span data-stu-id="a179c-133">id</span></span>|<span data-ttu-id="a179c-134">String</span><span class="sxs-lookup"><span data-stu-id="a179c-134">String</span></span>|<span data-ttu-id="a179c-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="a179c-135">The key of the entity.</span></span>|
|<span data-ttu-id="a179c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a179c-136">displayName</span></span>|<span data-ttu-id="a179c-137">Строка</span><span class="sxs-lookup"><span data-stu-id="a179c-137">String</span></span>|<span data-ttu-id="a179c-138">Имя категории электронная книга.</span><span class="sxs-lookup"><span data-stu-id="a179c-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="a179c-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a179c-139">lastModifiedDateTime</span></span>|<span data-ttu-id="a179c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a179c-140">DateTimeOffset</span></span>|<span data-ttu-id="a179c-141">Дата и время последнего изменения ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="a179c-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a179c-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="a179c-142">Response</span></span>
<span data-ttu-id="a179c-143">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [managedEBookCategory](../resources/intune-books-managedebookcategory.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="a179c-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a179c-144">Пример</span><span class="sxs-lookup"><span data-stu-id="a179c-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="a179c-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="a179c-145">Request</span></span>
<span data-ttu-id="a179c-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a179c-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="a179c-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="a179c-147">Response</span></span>
<span data-ttu-id="a179c-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="a179c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





