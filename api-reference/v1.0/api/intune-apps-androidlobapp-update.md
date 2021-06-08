---
title: Update androidLobApp
description: Обновление свойств объекта androidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df75bcedcdad698bb48a607c2833cf5149e9af6f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757705"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="e38f4-103">Update androidLobApp</span><span class="sxs-lookup"><span data-stu-id="e38f4-103">Update androidLobApp</span></span>

<span data-ttu-id="e38f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e38f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e38f4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e38f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e38f4-106">Обновление свойств объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e38f4-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="e38f4-107">Prerequisites</span></span>
<span data-ttu-id="e38f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e38f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e38f4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e38f4-110">Permission type</span></span>|<span data-ttu-id="e38f4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e38f4-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e38f4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e38f4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e38f4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e38f4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e38f4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e38f4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e38f4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e38f4-115">Not supported.</span></span>|
|<span data-ttu-id="e38f4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="e38f4-116">Application</span></span>|<span data-ttu-id="e38f4-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e38f4-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e38f4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e38f4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="e38f4-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="e38f4-119">Request headers</span></span>
|<span data-ttu-id="e38f4-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e38f4-120">Header</span></span>|<span data-ttu-id="e38f4-121">Значение</span><span class="sxs-lookup"><span data-stu-id="e38f4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e38f4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e38f4-122">Authorization</span></span>|<span data-ttu-id="e38f4-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e38f4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e38f4-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e38f4-124">Accept</span></span>|<span data-ttu-id="e38f4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e38f4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e38f4-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e38f4-126">Request body</span></span>
<span data-ttu-id="e38f4-127">В теле запроса добавьте представление объекта [androidLobApp](../resources/intune-apps-androidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e38f4-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="e38f4-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="e38f4-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="e38f4-129">Property</span></span>|<span data-ttu-id="e38f4-130">Тип</span><span class="sxs-lookup"><span data-stu-id="e38f4-130">Type</span></span>|<span data-ttu-id="e38f4-131">Описание</span><span class="sxs-lookup"><span data-stu-id="e38f4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e38f4-132">id</span><span class="sxs-lookup"><span data-stu-id="e38f4-132">id</span></span>|<span data-ttu-id="e38f4-133">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-133">String</span></span>|<span data-ttu-id="e38f4-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="e38f4-134">Key of the entity.</span></span> <span data-ttu-id="e38f4-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e38f4-136">displayName</span></span>|<span data-ttu-id="e38f4-137">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-137">String</span></span>|<span data-ttu-id="e38f4-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="e38f4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e38f4-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-140">description</span><span class="sxs-lookup"><span data-stu-id="e38f4-140">description</span></span>|<span data-ttu-id="e38f4-141">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-141">String</span></span>|<span data-ttu-id="e38f4-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="e38f4-142">The description of the app.</span></span> <span data-ttu-id="e38f4-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e38f4-144">publisher</span></span>|<span data-ttu-id="e38f4-145">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-145">String</span></span>|<span data-ttu-id="e38f4-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="e38f4-146">The publisher of the app.</span></span> <span data-ttu-id="e38f4-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e38f4-148">largeIcon</span></span>|[<span data-ttu-id="e38f4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e38f4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e38f4-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="e38f4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e38f4-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e38f4-152">createdDateTime</span></span>|<span data-ttu-id="e38f4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e38f4-153">DateTimeOffset</span></span>|<span data-ttu-id="e38f4-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="e38f4-154">The date and time the app was created.</span></span> <span data-ttu-id="e38f4-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e38f4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e38f4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e38f4-157">DateTimeOffset</span></span>|<span data-ttu-id="e38f4-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="e38f4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e38f4-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e38f4-160">isFeatured</span></span>|<span data-ttu-id="e38f4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e38f4-161">Boolean</span></span>|<span data-ttu-id="e38f4-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e38f4-163">privacyInformationUrl</span></span>|<span data-ttu-id="e38f4-164">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-164">String</span></span>|<span data-ttu-id="e38f4-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="e38f4-165">The privacy statement Url.</span></span> <span data-ttu-id="e38f4-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e38f4-167">informationUrl</span></span>|<span data-ttu-id="e38f4-168">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-168">String</span></span>|<span data-ttu-id="e38f4-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="e38f4-169">The more information Url.</span></span> <span data-ttu-id="e38f4-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-171">owner</span><span class="sxs-lookup"><span data-stu-id="e38f4-171">owner</span></span>|<span data-ttu-id="e38f4-172">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-172">String</span></span>|<span data-ttu-id="e38f4-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="e38f4-173">The owner of the app.</span></span> <span data-ttu-id="e38f4-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-175">developer</span><span class="sxs-lookup"><span data-stu-id="e38f4-175">developer</span></span>|<span data-ttu-id="e38f4-176">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-176">String</span></span>|<span data-ttu-id="e38f4-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="e38f4-177">The developer of the app.</span></span> <span data-ttu-id="e38f4-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-179">notes</span><span class="sxs-lookup"><span data-stu-id="e38f4-179">notes</span></span>|<span data-ttu-id="e38f4-180">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-180">String</span></span>|<span data-ttu-id="e38f4-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="e38f4-181">Notes for the app.</span></span> <span data-ttu-id="e38f4-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e38f4-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="e38f4-183">publishingState</span></span>|[<span data-ttu-id="e38f4-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e38f4-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e38f4-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="e38f4-185">The publishing state for the app.</span></span> <span data-ttu-id="e38f4-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="e38f4-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e38f4-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e38f4-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="e38f4-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e38f4-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e38f4-189">committedContentVersion</span></span>|<span data-ttu-id="e38f4-190">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-190">String</span></span>|<span data-ttu-id="e38f4-191">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="e38f4-191">The internal committed content version.</span></span> <span data-ttu-id="e38f4-192">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e38f4-193">fileName</span><span class="sxs-lookup"><span data-stu-id="e38f4-193">fileName</span></span>|<span data-ttu-id="e38f4-194">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-194">String</span></span>|<span data-ttu-id="e38f4-195">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="e38f4-195">The name of the main Lob application file.</span></span> <span data-ttu-id="e38f4-196">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e38f4-197">size</span><span class="sxs-lookup"><span data-stu-id="e38f4-197">size</span></span>|<span data-ttu-id="e38f4-198">Int64</span><span class="sxs-lookup"><span data-stu-id="e38f4-198">Int64</span></span>|<span data-ttu-id="e38f4-199">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="e38f4-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="e38f4-200">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="e38f4-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="e38f4-201">packageId</span><span class="sxs-lookup"><span data-stu-id="e38f4-201">packageId</span></span>|<span data-ttu-id="e38f4-202">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-202">String</span></span>|<span data-ttu-id="e38f4-203">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="e38f4-203">The package identifier.</span></span>|
|<span data-ttu-id="e38f4-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e38f4-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="e38f4-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="e38f4-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="e38f4-206">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="e38f4-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="e38f4-207">versionName</span><span class="sxs-lookup"><span data-stu-id="e38f4-207">versionName</span></span>|<span data-ttu-id="e38f4-208">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-208">String</span></span>|<span data-ttu-id="e38f4-209">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="e38f4-209">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="e38f4-210">versionCode</span><span class="sxs-lookup"><span data-stu-id="e38f4-210">versionCode</span></span>|<span data-ttu-id="e38f4-211">String</span><span class="sxs-lookup"><span data-stu-id="e38f4-211">String</span></span>|<span data-ttu-id="e38f4-212">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="e38f4-212">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="e38f4-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="e38f4-213">Response</span></span>
<span data-ttu-id="e38f4-214">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e38f4-214">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e38f4-215">Пример</span><span class="sxs-lookup"><span data-stu-id="e38f4-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="e38f4-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="e38f4-216">Request</span></span>
<span data-ttu-id="e38f4-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e38f4-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1115

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="e38f4-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="e38f4-218">Response</span></span>
<span data-ttu-id="e38f4-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e38f4-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1287

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
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
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v10_0": true,
    "v11_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```




