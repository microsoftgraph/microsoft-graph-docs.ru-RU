---
title: Обновление windowsPhoneXAP
description: Обновление свойства объекта windowsPhoneXAP.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eb99e9a504121d062eb4127f6137752f28c9d2bb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823158"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="30e22-103">Обновление windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="30e22-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="30e22-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="30e22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30e22-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30e22-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="30e22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30e22-107">Обновление свойства объекта [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="30e22-107">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30e22-108">Необходимые компоненты</span><span class="sxs-lookup"><span data-stu-id="30e22-108">Prerequisites</span></span>
<span data-ttu-id="30e22-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30e22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30e22-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="30e22-111">Permission type</span></span>|<span data-ttu-id="30e22-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="30e22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30e22-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="30e22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30e22-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30e22-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="30e22-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="30e22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30e22-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e22-116">Not supported.</span></span>|
|<span data-ttu-id="30e22-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="30e22-117">Application</span></span>|<span data-ttu-id="30e22-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="30e22-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30e22-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="30e22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="30e22-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="30e22-120">Request headers</span></span>
|<span data-ttu-id="30e22-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="30e22-121">Header</span></span>|<span data-ttu-id="30e22-122">Значение</span><span class="sxs-lookup"><span data-stu-id="30e22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30e22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="30e22-123">Authorization</span></span>|<span data-ttu-id="30e22-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="30e22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30e22-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30e22-125">Accept</span></span>|<span data-ttu-id="30e22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30e22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30e22-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="30e22-127">Request body</span></span>
<span data-ttu-id="30e22-128">В тексте запроса укажите представление JSON для объекта [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="30e22-128">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="30e22-129">В следующей таблице показаны свойства, которые необходимы для создания [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-129">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="30e22-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="30e22-130">Property</span></span>|<span data-ttu-id="30e22-131">Тип</span><span class="sxs-lookup"><span data-stu-id="30e22-131">Type</span></span>|<span data-ttu-id="30e22-132">Описание</span><span class="sxs-lookup"><span data-stu-id="30e22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30e22-133">id</span><span class="sxs-lookup"><span data-stu-id="30e22-133">id</span></span>|<span data-ttu-id="30e22-134">Строка</span><span class="sxs-lookup"><span data-stu-id="30e22-134">String</span></span>|<span data-ttu-id="30e22-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="30e22-135">Key of the entity.</span></span> <span data-ttu-id="30e22-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-137">displayName</span><span class="sxs-lookup"><span data-stu-id="30e22-137">displayName</span></span>|<span data-ttu-id="30e22-138">String</span><span class="sxs-lookup"><span data-stu-id="30e22-138">String</span></span>|<span data-ttu-id="30e22-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="30e22-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="30e22-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-141">описание</span><span class="sxs-lookup"><span data-stu-id="30e22-141">description</span></span>|<span data-ttu-id="30e22-142">String</span><span class="sxs-lookup"><span data-stu-id="30e22-142">String</span></span>|<span data-ttu-id="30e22-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="30e22-143">The description of the app.</span></span> <span data-ttu-id="30e22-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-145">publisher</span><span class="sxs-lookup"><span data-stu-id="30e22-145">publisher</span></span>|<span data-ttu-id="30e22-146">String</span><span class="sxs-lookup"><span data-stu-id="30e22-146">String</span></span>|<span data-ttu-id="30e22-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="30e22-147">The publisher of the app.</span></span> <span data-ttu-id="30e22-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="30e22-149">largeIcon</span></span>|[<span data-ttu-id="30e22-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="30e22-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="30e22-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="30e22-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="30e22-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="30e22-153">createdDateTime</span></span>|<span data-ttu-id="30e22-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30e22-154">DateTimeOffset</span></span>|<span data-ttu-id="30e22-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="30e22-155">The date and time the app was created.</span></span> <span data-ttu-id="30e22-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30e22-157">lastModifiedDateTime</span></span>|<span data-ttu-id="30e22-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30e22-158">DateTimeOffset</span></span>|<span data-ttu-id="30e22-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="30e22-159">The date and time the app was last modified.</span></span> <span data-ttu-id="30e22-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="30e22-161">isFeatured</span></span>|<span data-ttu-id="30e22-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="30e22-162">Boolean</span></span>|<span data-ttu-id="30e22-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="30e22-164">privacyInformationUrl</span></span>|<span data-ttu-id="30e22-165">String</span><span class="sxs-lookup"><span data-stu-id="30e22-165">String</span></span>|<span data-ttu-id="30e22-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="30e22-166">The privacy statement Url.</span></span> <span data-ttu-id="30e22-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="30e22-168">informationUrl</span></span>|<span data-ttu-id="30e22-169">String</span><span class="sxs-lookup"><span data-stu-id="30e22-169">String</span></span>|<span data-ttu-id="30e22-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="30e22-170">The more information Url.</span></span> <span data-ttu-id="30e22-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-172">owner</span><span class="sxs-lookup"><span data-stu-id="30e22-172">owner</span></span>|<span data-ttu-id="30e22-173">String</span><span class="sxs-lookup"><span data-stu-id="30e22-173">String</span></span>|<span data-ttu-id="30e22-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="30e22-174">The owner of the app.</span></span> <span data-ttu-id="30e22-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-176">developer</span><span class="sxs-lookup"><span data-stu-id="30e22-176">developer</span></span>|<span data-ttu-id="30e22-177">String</span><span class="sxs-lookup"><span data-stu-id="30e22-177">String</span></span>|<span data-ttu-id="30e22-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="30e22-178">The developer of the app.</span></span> <span data-ttu-id="30e22-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-180">notes</span><span class="sxs-lookup"><span data-stu-id="30e22-180">notes</span></span>|<span data-ttu-id="30e22-181">String</span><span class="sxs-lookup"><span data-stu-id="30e22-181">String</span></span>|<span data-ttu-id="30e22-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="30e22-182">Notes for the app.</span></span> <span data-ttu-id="30e22-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="30e22-184">uploadState</span></span>|<span data-ttu-id="30e22-185">Int32</span><span class="sxs-lookup"><span data-stu-id="30e22-185">Int32</span></span>|<span data-ttu-id="30e22-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="30e22-186">The upload state.</span></span> <span data-ttu-id="30e22-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="30e22-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="30e22-188">publishingState</span></span>|[<span data-ttu-id="30e22-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="30e22-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="30e22-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="30e22-190">The publishing state for the app.</span></span> <span data-ttu-id="30e22-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="30e22-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="30e22-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="30e22-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="30e22-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="30e22-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="30e22-194">committedContentVersion</span></span>|<span data-ttu-id="30e22-195">String</span><span class="sxs-lookup"><span data-stu-id="30e22-195">String</span></span>|<span data-ttu-id="30e22-196">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="30e22-196">The internal committed content version.</span></span> <span data-ttu-id="30e22-197">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30e22-198">fileName</span><span class="sxs-lookup"><span data-stu-id="30e22-198">fileName</span></span>|<span data-ttu-id="30e22-199">String</span><span class="sxs-lookup"><span data-stu-id="30e22-199">String</span></span>|<span data-ttu-id="30e22-200">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="30e22-200">The name of the main Lob application file.</span></span> <span data-ttu-id="30e22-201">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30e22-202">size</span><span class="sxs-lookup"><span data-stu-id="30e22-202">size</span></span>|<span data-ttu-id="30e22-203">Int64</span><span class="sxs-lookup"><span data-stu-id="30e22-203">Int64</span></span>|<span data-ttu-id="30e22-204">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="30e22-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="30e22-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="30e22-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="30e22-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30e22-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="30e22-207">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="30e22-207">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="30e22-208">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="30e22-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="30e22-209">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="30e22-209">productIdentifier</span></span>|<span data-ttu-id="30e22-210">Строка</span><span class="sxs-lookup"><span data-stu-id="30e22-210">String</span></span>|<span data-ttu-id="30e22-211">Идентификатор продукта.</span><span class="sxs-lookup"><span data-stu-id="30e22-211">The Product Identifier.</span></span>|
|<span data-ttu-id="30e22-212">identityVersion</span><span class="sxs-lookup"><span data-stu-id="30e22-212">identityVersion</span></span>|<span data-ttu-id="30e22-213">String</span><span class="sxs-lookup"><span data-stu-id="30e22-213">String</span></span>|<span data-ttu-id="30e22-214">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="30e22-214">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="30e22-215">Ответ</span><span class="sxs-lookup"><span data-stu-id="30e22-215">Response</span></span>
<span data-ttu-id="30e22-216">Успешно завершена, этот метод возвращает `200 OK` код ответа и обновленные [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) объекта в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="30e22-216">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30e22-217">Пример</span><span class="sxs-lookup"><span data-stu-id="30e22-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="30e22-218">Запрос</span><span class="sxs-lookup"><span data-stu-id="30e22-218">Request</span></span>
<span data-ttu-id="30e22-219">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="30e22-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1089

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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="30e22-220">Ответ</span><span class="sxs-lookup"><span data-stu-id="30e22-220">Response</span></span>
<span data-ttu-id="30e22-p120">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="30e22-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1251

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```





