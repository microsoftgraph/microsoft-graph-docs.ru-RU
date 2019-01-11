---
title: Update microsoftStoreForBusinessApp
description: Обновление свойств объекта microsoftStoreForBusinessApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a4e54e3d7b38471b4c9d86cc50cb6b7536205008
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843136"
---
# <a name="update-microsoftstoreforbusinessapp"></a><span data-ttu-id="f1cc3-103">Update microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="f1cc3-103">Update microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="f1cc3-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1cc3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1cc3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1cc3-107">Обновление свойств объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-107">Update the properties of a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1cc3-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="f1cc3-108">Prerequisites</span></span>
<span data-ttu-id="f1cc3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1cc3-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1cc3-111">Permission type</span></span>|<span data-ttu-id="f1cc3-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1cc3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1cc3-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1cc3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1cc3-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1cc3-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f1cc3-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1cc3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1cc3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-116">Not supported.</span></span>|
|<span data-ttu-id="f1cc3-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f1cc3-117">Application</span></span>|<span data-ttu-id="f1cc3-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1cc3-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1cc3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f1cc3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1cc3-120">Request headers</span></span>
|<span data-ttu-id="f1cc3-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1cc3-121">Header</span></span>|<span data-ttu-id="f1cc3-122">Значение</span><span class="sxs-lookup"><span data-stu-id="f1cc3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1cc3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1cc3-123">Authorization</span></span>|<span data-ttu-id="f1cc3-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="f1cc3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1cc3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f1cc3-125">Accept</span></span>|<span data-ttu-id="f1cc3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1cc3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1cc3-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="f1cc3-127">Request body</span></span>
<span data-ttu-id="f1cc3-128">В теле запроса добавьте представление объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

<span data-ttu-id="f1cc3-129">Ниже показаны свойства, которые необходимо указывать при создании объекта [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md).</span></span>

|<span data-ttu-id="f1cc3-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="f1cc3-130">Property</span></span>|<span data-ttu-id="f1cc3-131">Тип</span><span class="sxs-lookup"><span data-stu-id="f1cc3-131">Type</span></span>|<span data-ttu-id="f1cc3-132">Описание</span><span class="sxs-lookup"><span data-stu-id="f1cc3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1cc3-133">id</span><span class="sxs-lookup"><span data-stu-id="f1cc3-133">id</span></span>|<span data-ttu-id="f1cc3-134">Строка</span><span class="sxs-lookup"><span data-stu-id="f1cc3-134">String</span></span>|<span data-ttu-id="f1cc3-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-135">Key of the entity.</span></span> <span data-ttu-id="f1cc3-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f1cc3-137">displayName</span></span>|<span data-ttu-id="f1cc3-138">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-138">String</span></span>|<span data-ttu-id="f1cc3-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f1cc3-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-141">описание</span><span class="sxs-lookup"><span data-stu-id="f1cc3-141">description</span></span>|<span data-ttu-id="f1cc3-142">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-142">String</span></span>|<span data-ttu-id="f1cc3-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-143">The description of the app.</span></span> <span data-ttu-id="f1cc3-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f1cc3-145">publisher</span></span>|<span data-ttu-id="f1cc3-146">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-146">String</span></span>|<span data-ttu-id="f1cc3-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-147">The publisher of the app.</span></span> <span data-ttu-id="f1cc3-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f1cc3-149">largeIcon</span></span>|[<span data-ttu-id="f1cc3-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f1cc3-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f1cc3-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f1cc3-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1cc3-153">createdDateTime</span></span>|<span data-ttu-id="f1cc3-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1cc3-154">DateTimeOffset</span></span>|<span data-ttu-id="f1cc3-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-155">The date and time the app was created.</span></span> <span data-ttu-id="f1cc3-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1cc3-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f1cc3-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1cc3-158">DateTimeOffset</span></span>|<span data-ttu-id="f1cc3-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f1cc3-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f1cc3-161">isFeatured</span></span>|<span data-ttu-id="f1cc3-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1cc3-162">Boolean</span></span>|<span data-ttu-id="f1cc3-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f1cc3-164">privacyInformationUrl</span></span>|<span data-ttu-id="f1cc3-165">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-165">String</span></span>|<span data-ttu-id="f1cc3-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-166">The privacy statement Url.</span></span> <span data-ttu-id="f1cc3-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f1cc3-168">informationUrl</span></span>|<span data-ttu-id="f1cc3-169">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-169">String</span></span>|<span data-ttu-id="f1cc3-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-170">The more information Url.</span></span> <span data-ttu-id="f1cc3-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-172">owner</span><span class="sxs-lookup"><span data-stu-id="f1cc3-172">owner</span></span>|<span data-ttu-id="f1cc3-173">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-173">String</span></span>|<span data-ttu-id="f1cc3-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-174">The owner of the app.</span></span> <span data-ttu-id="f1cc3-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-176">developer</span><span class="sxs-lookup"><span data-stu-id="f1cc3-176">developer</span></span>|<span data-ttu-id="f1cc3-177">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-177">String</span></span>|<span data-ttu-id="f1cc3-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-178">The developer of the app.</span></span> <span data-ttu-id="f1cc3-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-180">notes</span><span class="sxs-lookup"><span data-stu-id="f1cc3-180">notes</span></span>|<span data-ttu-id="f1cc3-181">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-181">String</span></span>|<span data-ttu-id="f1cc3-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-182">Notes for the app.</span></span> <span data-ttu-id="f1cc3-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f1cc3-184">uploadState</span></span>|<span data-ttu-id="f1cc3-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f1cc3-185">Int32</span></span>|<span data-ttu-id="f1cc3-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-186">The upload state.</span></span> <span data-ttu-id="f1cc3-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1cc3-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f1cc3-188">publishingState</span></span>|[<span data-ttu-id="f1cc3-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f1cc3-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f1cc3-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-190">The publishing state for the app.</span></span> <span data-ttu-id="f1cc3-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f1cc3-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1cc3-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f1cc3-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f1cc3-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f1cc3-194">usedLicenseCount</span></span>|<span data-ttu-id="f1cc3-195">Int32</span><span class="sxs-lookup"><span data-stu-id="f1cc3-195">Int32</span></span>|<span data-ttu-id="f1cc3-196">Количество используемых лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-196">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="f1cc3-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f1cc3-197">totalLicenseCount</span></span>|<span data-ttu-id="f1cc3-198">Int32</span><span class="sxs-lookup"><span data-stu-id="f1cc3-198">Int32</span></span>|<span data-ttu-id="f1cc3-199">Общее количество лицензий Microsoft Store для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-199">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="f1cc3-200">productKey</span><span class="sxs-lookup"><span data-stu-id="f1cc3-200">productKey</span></span>|<span data-ttu-id="f1cc3-201">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-201">String</span></span>|<span data-ttu-id="f1cc3-202">Ключ продукта для приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-202">The app product key</span></span>|
|<span data-ttu-id="f1cc3-203">licenseType</span><span class="sxs-lookup"><span data-stu-id="f1cc3-203">licenseType</span></span>|[<span data-ttu-id="f1cc3-204">microsoftStoreForBusinessLicenseType</span><span class="sxs-lookup"><span data-stu-id="f1cc3-204">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="f1cc3-205">Тип лицензии приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-205">The app license type.</span></span> <span data-ttu-id="f1cc3-206">Возможные значения: `offline`, `online`.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-206">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="f1cc3-207">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="f1cc3-207">packageIdentityName</span></span>|<span data-ttu-id="f1cc3-208">String</span><span class="sxs-lookup"><span data-stu-id="f1cc3-208">String</span></span>|<span data-ttu-id="f1cc3-209">Идентификатор пакета приложения.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-209">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="f1cc3-210">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1cc3-210">Response</span></span>
<span data-ttu-id="f1cc3-211">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-211">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1cc3-212">Пример</span><span class="sxs-lookup"><span data-stu-id="f1cc3-212">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1cc3-213">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1cc3-213">Request</span></span>
<span data-ttu-id="f1cc3-214">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-214">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 788

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="f1cc3-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="f1cc3-215">Response</span></span>
<span data-ttu-id="f1cc3-p118">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="f1cc3-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 963

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```





