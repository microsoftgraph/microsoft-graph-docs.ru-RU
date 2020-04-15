---
title: Create androidLobApp
description: Создание нового объекта androidLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f67300d100c3487259ae54e9322ffef70256a595
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463988"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="45bca-103">Create androidLobApp</span><span class="sxs-lookup"><span data-stu-id="45bca-103">Create androidLobApp</span></span>

<span data-ttu-id="45bca-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45bca-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45bca-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="45bca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45bca-106">Создание нового объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-106">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="45bca-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="45bca-107">Prerequisites</span></span>
<span data-ttu-id="45bca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45bca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45bca-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45bca-110">Permission type</span></span>|<span data-ttu-id="45bca-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="45bca-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45bca-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45bca-112">Delegated (work or school account)</span></span>|<span data-ttu-id="45bca-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45bca-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45bca-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45bca-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45bca-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45bca-115">Not supported.</span></span>|
|<span data-ttu-id="45bca-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45bca-116">Application</span></span>|<span data-ttu-id="45bca-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="45bca-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45bca-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45bca-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="45bca-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="45bca-119">Request headers</span></span>
|<span data-ttu-id="45bca-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="45bca-120">Header</span></span>|<span data-ttu-id="45bca-121">Значение</span><span class="sxs-lookup"><span data-stu-id="45bca-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45bca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="45bca-122">Authorization</span></span>|<span data-ttu-id="45bca-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45bca-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45bca-124">Accept</span><span class="sxs-lookup"><span data-stu-id="45bca-124">Accept</span></span>|<span data-ttu-id="45bca-125">application/json</span><span class="sxs-lookup"><span data-stu-id="45bca-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45bca-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45bca-126">Request body</span></span>
<span data-ttu-id="45bca-127">В теле запроса добавьте представление объекта androidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="45bca-127">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="45bca-128">Ниже показаны свойства, которые необходимо указывать при создании объекта androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="45bca-128">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="45bca-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="45bca-129">Property</span></span>|<span data-ttu-id="45bca-130">Тип</span><span class="sxs-lookup"><span data-stu-id="45bca-130">Type</span></span>|<span data-ttu-id="45bca-131">Описание</span><span class="sxs-lookup"><span data-stu-id="45bca-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45bca-132">id</span><span class="sxs-lookup"><span data-stu-id="45bca-132">id</span></span>|<span data-ttu-id="45bca-133">Строка</span><span class="sxs-lookup"><span data-stu-id="45bca-133">String</span></span>|<span data-ttu-id="45bca-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="45bca-134">Key of the entity.</span></span> <span data-ttu-id="45bca-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-136">displayName</span><span class="sxs-lookup"><span data-stu-id="45bca-136">displayName</span></span>|<span data-ttu-id="45bca-137">Строка</span><span class="sxs-lookup"><span data-stu-id="45bca-137">String</span></span>|<span data-ttu-id="45bca-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="45bca-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="45bca-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-140">description</span><span class="sxs-lookup"><span data-stu-id="45bca-140">description</span></span>|<span data-ttu-id="45bca-141">Строка</span><span class="sxs-lookup"><span data-stu-id="45bca-141">String</span></span>|<span data-ttu-id="45bca-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="45bca-142">The description of the app.</span></span> <span data-ttu-id="45bca-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-144">publisher</span><span class="sxs-lookup"><span data-stu-id="45bca-144">publisher</span></span>|<span data-ttu-id="45bca-145">String</span><span class="sxs-lookup"><span data-stu-id="45bca-145">String</span></span>|<span data-ttu-id="45bca-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="45bca-146">The publisher of the app.</span></span> <span data-ttu-id="45bca-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="45bca-148">largeIcon</span></span>|[<span data-ttu-id="45bca-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="45bca-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="45bca-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="45bca-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="45bca-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="45bca-152">createdDateTime</span></span>|<span data-ttu-id="45bca-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45bca-153">DateTimeOffset</span></span>|<span data-ttu-id="45bca-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="45bca-154">The date and time the app was created.</span></span> <span data-ttu-id="45bca-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="45bca-156">lastModifiedDateTime</span></span>|<span data-ttu-id="45bca-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45bca-157">DateTimeOffset</span></span>|<span data-ttu-id="45bca-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="45bca-158">The date and time the app was last modified.</span></span> <span data-ttu-id="45bca-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="45bca-160">isFeatured</span></span>|<span data-ttu-id="45bca-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="45bca-161">Boolean</span></span>|<span data-ttu-id="45bca-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="45bca-163">privacyInformationUrl</span></span>|<span data-ttu-id="45bca-164">String</span><span class="sxs-lookup"><span data-stu-id="45bca-164">String</span></span>|<span data-ttu-id="45bca-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="45bca-165">The privacy statement Url.</span></span> <span data-ttu-id="45bca-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="45bca-167">informationUrl</span></span>|<span data-ttu-id="45bca-168">String</span><span class="sxs-lookup"><span data-stu-id="45bca-168">String</span></span>|<span data-ttu-id="45bca-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="45bca-169">The more information Url.</span></span> <span data-ttu-id="45bca-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-171">owner</span><span class="sxs-lookup"><span data-stu-id="45bca-171">owner</span></span>|<span data-ttu-id="45bca-172">String</span><span class="sxs-lookup"><span data-stu-id="45bca-172">String</span></span>|<span data-ttu-id="45bca-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="45bca-173">The owner of the app.</span></span> <span data-ttu-id="45bca-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-175">developer</span><span class="sxs-lookup"><span data-stu-id="45bca-175">developer</span></span>|<span data-ttu-id="45bca-176">String</span><span class="sxs-lookup"><span data-stu-id="45bca-176">String</span></span>|<span data-ttu-id="45bca-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="45bca-177">The developer of the app.</span></span> <span data-ttu-id="45bca-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-179">notes</span><span class="sxs-lookup"><span data-stu-id="45bca-179">notes</span></span>|<span data-ttu-id="45bca-180">String</span><span class="sxs-lookup"><span data-stu-id="45bca-180">String</span></span>|<span data-ttu-id="45bca-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="45bca-181">Notes for the app.</span></span> <span data-ttu-id="45bca-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="45bca-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="45bca-183">publishingState</span></span>|[<span data-ttu-id="45bca-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="45bca-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="45bca-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="45bca-185">The publishing state for the app.</span></span> <span data-ttu-id="45bca-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="45bca-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="45bca-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="45bca-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="45bca-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="45bca-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="45bca-189">committedContentVersion</span></span>|<span data-ttu-id="45bca-190">String</span><span class="sxs-lookup"><span data-stu-id="45bca-190">String</span></span>|<span data-ttu-id="45bca-191">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="45bca-191">The internal committed content version.</span></span> <span data-ttu-id="45bca-192">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="45bca-193">fileName</span><span class="sxs-lookup"><span data-stu-id="45bca-193">fileName</span></span>|<span data-ttu-id="45bca-194">String</span><span class="sxs-lookup"><span data-stu-id="45bca-194">String</span></span>|<span data-ttu-id="45bca-195">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="45bca-195">The name of the main Lob application file.</span></span> <span data-ttu-id="45bca-196">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="45bca-197">size</span><span class="sxs-lookup"><span data-stu-id="45bca-197">size</span></span>|<span data-ttu-id="45bca-198">Int64</span><span class="sxs-lookup"><span data-stu-id="45bca-198">Int64</span></span>|<span data-ttu-id="45bca-199">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="45bca-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="45bca-200">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="45bca-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="45bca-201">packageId</span><span class="sxs-lookup"><span data-stu-id="45bca-201">packageId</span></span>|<span data-ttu-id="45bca-202">String</span><span class="sxs-lookup"><span data-stu-id="45bca-202">String</span></span>|<span data-ttu-id="45bca-203">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="45bca-203">The package identifier.</span></span>|
|<span data-ttu-id="45bca-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="45bca-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="45bca-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="45bca-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="45bca-206">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="45bca-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="45bca-207">versionName</span><span class="sxs-lookup"><span data-stu-id="45bca-207">versionName</span></span>|<span data-ttu-id="45bca-208">String</span><span class="sxs-lookup"><span data-stu-id="45bca-208">String</span></span>|<span data-ttu-id="45bca-209">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="45bca-209">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="45bca-210">versionCode</span><span class="sxs-lookup"><span data-stu-id="45bca-210">versionCode</span></span>|<span data-ttu-id="45bca-211">String</span><span class="sxs-lookup"><span data-stu-id="45bca-211">String</span></span>|<span data-ttu-id="45bca-212">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="45bca-212">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="45bca-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="45bca-213">Response</span></span>
<span data-ttu-id="45bca-214">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="45bca-214">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45bca-215">Пример</span><span class="sxs-lookup"><span data-stu-id="45bca-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="45bca-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="45bca-216">Request</span></span>
<span data-ttu-id="45bca-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45bca-217">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1075

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
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="45bca-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="45bca-218">Response</span></span>
<span data-ttu-id="45bca-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="45bca-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1247

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
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```






