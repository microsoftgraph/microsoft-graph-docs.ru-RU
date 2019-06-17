---
title: Обновление Манажедебуккатегори
description: Обновление свойств объекта Манажедебуккатегори.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4a9f9ea4d7f8c53c5dc35aed552edb6d7bbea11
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972146"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="43118-103">Обновление Манажедебуккатегори</span><span class="sxs-lookup"><span data-stu-id="43118-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="43118-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43118-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43118-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="43118-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43118-106">Обновление свойств объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="43118-106">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43118-107">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="43118-107">Prerequisites</span></span>
<span data-ttu-id="43118-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43118-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43118-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43118-110">Permission type</span></span>|<span data-ttu-id="43118-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="43118-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43118-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43118-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43118-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43118-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43118-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43118-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43118-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43118-115">Not supported.</span></span>|
|<span data-ttu-id="43118-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="43118-116">Application</span></span>|<span data-ttu-id="43118-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43118-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43118-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43118-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="43118-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43118-119">Request headers</span></span>
|<span data-ttu-id="43118-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="43118-120">Header</span></span>|<span data-ttu-id="43118-121">Значение</span><span class="sxs-lookup"><span data-stu-id="43118-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43118-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43118-122">Authorization</span></span>|<span data-ttu-id="43118-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43118-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43118-124">Accept</span><span class="sxs-lookup"><span data-stu-id="43118-124">Accept</span></span>|<span data-ttu-id="43118-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43118-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43118-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="43118-126">Request body</span></span>
<span data-ttu-id="43118-127">В тексте запроса добавьте представление объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="43118-127">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="43118-128">В следующей таблице приведены свойства, необходимые при создании [манажедебуккатегори](../resources/intune-books-managedebookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="43118-128">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="43118-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="43118-129">Property</span></span>|<span data-ttu-id="43118-130">Тип</span><span class="sxs-lookup"><span data-stu-id="43118-130">Type</span></span>|<span data-ttu-id="43118-131">Описание</span><span class="sxs-lookup"><span data-stu-id="43118-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43118-132">id</span><span class="sxs-lookup"><span data-stu-id="43118-132">id</span></span>|<span data-ttu-id="43118-133">String</span><span class="sxs-lookup"><span data-stu-id="43118-133">String</span></span>|<span data-ttu-id="43118-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="43118-134">The key of the entity.</span></span>|
|<span data-ttu-id="43118-135">displayName</span><span class="sxs-lookup"><span data-stu-id="43118-135">displayName</span></span>|<span data-ttu-id="43118-136">Строка</span><span class="sxs-lookup"><span data-stu-id="43118-136">String</span></span>|<span data-ttu-id="43118-137">Имя категории электронной книги.</span><span class="sxs-lookup"><span data-stu-id="43118-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="43118-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43118-138">lastModifiedDateTime</span></span>|<span data-ttu-id="43118-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43118-139">DateTimeOffset</span></span>|<span data-ttu-id="43118-140">Дата и время последнего изменения Манажедебуккатегори.</span><span class="sxs-lookup"><span data-stu-id="43118-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="43118-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="43118-141">Response</span></span>
<span data-ttu-id="43118-142">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="43118-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43118-143">Пример</span><span class="sxs-lookup"><span data-stu-id="43118-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="43118-144">Запрос</span><span class="sxs-lookup"><span data-stu-id="43118-144">Request</span></span>
<span data-ttu-id="43118-145">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="43118-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="43118-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="43118-146">Response</span></span>
<span data-ttu-id="43118-p102">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="43118-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





