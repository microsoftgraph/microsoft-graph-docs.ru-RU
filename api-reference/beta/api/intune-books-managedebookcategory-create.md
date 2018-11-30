---
title: Создание managedEBookCategory
description: Создание нового объекта managedEBookCategory.
ms.openlocfilehash: 8750e8c520e3a48b2da93d05b9f701c7760b6a15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081189"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="c5ccb-103">Создание managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="c5ccb-103">Create managedEBookCategory</span></span>

> <span data-ttu-id="c5ccb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5ccb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5ccb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5ccb-107">Создание нового объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="c5ccb-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c5ccb-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="c5ccb-108">Prerequisites</span></span>
<span data-ttu-id="c5ccb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c5ccb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5ccb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c5ccb-111">Permission type</span></span>|<span data-ttu-id="c5ccb-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c5ccb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c5ccb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c5ccb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c5ccb-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5ccb-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c5ccb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c5ccb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c5ccb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-116">Not supported.</span></span>|
|<span data-ttu-id="c5ccb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c5ccb-117">Application</span></span>|<span data-ttu-id="c5ccb-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c5ccb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c5ccb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="c5ccb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c5ccb-120">Request headers</span></span>
|<span data-ttu-id="c5ccb-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c5ccb-121">Header</span></span>|<span data-ttu-id="c5ccb-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c5ccb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c5ccb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5ccb-123">Authorization</span></span>|<span data-ttu-id="c5ccb-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c5ccb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c5ccb-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c5ccb-125">Accept</span></span>|<span data-ttu-id="c5ccb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c5ccb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c5ccb-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c5ccb-127">Request body</span></span>
<span data-ttu-id="c5ccb-128">В тексте запроса укажите представление JSON для объекта managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="c5ccb-129">В следующей таблице показаны свойства, которые необходимы для создания managedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="c5ccb-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c5ccb-130">Property</span></span>|<span data-ttu-id="c5ccb-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c5ccb-131">Type</span></span>|<span data-ttu-id="c5ccb-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c5ccb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5ccb-133">id</span><span class="sxs-lookup"><span data-stu-id="c5ccb-133">id</span></span>|<span data-ttu-id="c5ccb-134">String</span><span class="sxs-lookup"><span data-stu-id="c5ccb-134">String</span></span>|<span data-ttu-id="c5ccb-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-135">The key of the entity.</span></span>|
|<span data-ttu-id="c5ccb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="c5ccb-136">displayName</span></span>|<span data-ttu-id="c5ccb-137">String</span><span class="sxs-lookup"><span data-stu-id="c5ccb-137">String</span></span>|<span data-ttu-id="c5ccb-138">Имя категории электронная книга.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="c5ccb-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5ccb-139">lastModifiedDateTime</span></span>|<span data-ttu-id="c5ccb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5ccb-140">DateTimeOffset</span></span>|<span data-ttu-id="c5ccb-141">Дата и время последнего изменения ManagedEBookCategory.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="c5ccb-142">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5ccb-142">Response</span></span>
<span data-ttu-id="c5ccb-143">Успешно завершена, этот метод возвращает `201 Created` код ответа и объект [managedEBookCategory](../resources/intune-books-managedebookcategory.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5ccb-144">Пример</span><span class="sxs-lookup"><span data-stu-id="c5ccb-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="c5ccb-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="c5ccb-145">Request</span></span>
<span data-ttu-id="c5ccb-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c5ccb-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="c5ccb-147">Ответ</span><span class="sxs-lookup"><span data-stu-id="c5ccb-147">Response</span></span>
<span data-ttu-id="c5ccb-p103">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="c5ccb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```





