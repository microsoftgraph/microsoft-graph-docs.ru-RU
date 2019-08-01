---
title: Create androidLobApp
description: Создание нового объекта androidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a399549a624b0e72604637673c4ca86e7ff4b590
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014349"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="0faa7-103">Create androidLobApp</span><span class="sxs-lookup"><span data-stu-id="0faa7-103">Create androidLobApp</span></span>

> <span data-ttu-id="0faa7-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0faa7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0faa7-105">Создание нового объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-105">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0faa7-106">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="0faa7-106">Prerequisites</span></span>
<span data-ttu-id="0faa7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0faa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0faa7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0faa7-109">Permission type</span></span>|<span data-ttu-id="0faa7-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="0faa7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0faa7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0faa7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0faa7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0faa7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0faa7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0faa7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0faa7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0faa7-114">Not supported.</span></span>|
|<span data-ttu-id="0faa7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0faa7-115">Application</span></span>|<span data-ttu-id="0faa7-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0faa7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0faa7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0faa7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0faa7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0faa7-118">Request headers</span></span>
|<span data-ttu-id="0faa7-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="0faa7-119">Header</span></span>|<span data-ttu-id="0faa7-120">Значение</span><span class="sxs-lookup"><span data-stu-id="0faa7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0faa7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0faa7-121">Authorization</span></span>|<span data-ttu-id="0faa7-122">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0faa7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0faa7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0faa7-123">Accept</span></span>|<span data-ttu-id="0faa7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0faa7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0faa7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0faa7-125">Request body</span></span>
<span data-ttu-id="0faa7-126">В теле запроса добавьте представление объекта androidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0faa7-126">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="0faa7-127">Ниже показаны свойства, которые необходимо указывать при создании объекта androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="0faa7-127">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="0faa7-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="0faa7-128">Property</span></span>|<span data-ttu-id="0faa7-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0faa7-129">Type</span></span>|<span data-ttu-id="0faa7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="0faa7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0faa7-131">id</span><span class="sxs-lookup"><span data-stu-id="0faa7-131">id</span></span>|<span data-ttu-id="0faa7-132">Строка</span><span class="sxs-lookup"><span data-stu-id="0faa7-132">String</span></span>|<span data-ttu-id="0faa7-133">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="0faa7-133">Key of the entity.</span></span> <span data-ttu-id="0faa7-134">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="0faa7-135">displayName</span></span>|<span data-ttu-id="0faa7-136">Строка</span><span class="sxs-lookup"><span data-stu-id="0faa7-136">String</span></span>|<span data-ttu-id="0faa7-137">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="0faa7-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0faa7-138">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-139">description</span><span class="sxs-lookup"><span data-stu-id="0faa7-139">description</span></span>|<span data-ttu-id="0faa7-140">Строка</span><span class="sxs-lookup"><span data-stu-id="0faa7-140">String</span></span>|<span data-ttu-id="0faa7-141">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="0faa7-141">The description of the app.</span></span> <span data-ttu-id="0faa7-142">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-143">publisher</span><span class="sxs-lookup"><span data-stu-id="0faa7-143">publisher</span></span>|<span data-ttu-id="0faa7-144">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-144">String</span></span>|<span data-ttu-id="0faa7-145">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="0faa7-145">The publisher of the app.</span></span> <span data-ttu-id="0faa7-146">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0faa7-147">largeIcon</span></span>|[<span data-ttu-id="0faa7-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0faa7-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0faa7-149">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="0faa7-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0faa7-150">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0faa7-151">createdDateTime</span></span>|<span data-ttu-id="0faa7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0faa7-152">DateTimeOffset</span></span>|<span data-ttu-id="0faa7-153">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="0faa7-153">The date and time the app was created.</span></span> <span data-ttu-id="0faa7-154">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0faa7-155">lastModifiedDateTime</span></span>|<span data-ttu-id="0faa7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0faa7-156">DateTimeOffset</span></span>|<span data-ttu-id="0faa7-157">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="0faa7-157">The date and time the app was last modified.</span></span> <span data-ttu-id="0faa7-158">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0faa7-159">isFeatured</span></span>|<span data-ttu-id="0faa7-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="0faa7-160">Boolean</span></span>|<span data-ttu-id="0faa7-161">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0faa7-162">privacyInformationUrl</span></span>|<span data-ttu-id="0faa7-163">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-163">String</span></span>|<span data-ttu-id="0faa7-164">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="0faa7-164">The privacy statement Url.</span></span> <span data-ttu-id="0faa7-165">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0faa7-166">informationUrl</span></span>|<span data-ttu-id="0faa7-167">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-167">String</span></span>|<span data-ttu-id="0faa7-168">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="0faa7-168">The more information Url.</span></span> <span data-ttu-id="0faa7-169">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-170">owner</span><span class="sxs-lookup"><span data-stu-id="0faa7-170">owner</span></span>|<span data-ttu-id="0faa7-171">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-171">String</span></span>|<span data-ttu-id="0faa7-172">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="0faa7-172">The owner of the app.</span></span> <span data-ttu-id="0faa7-173">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-174">developer</span><span class="sxs-lookup"><span data-stu-id="0faa7-174">developer</span></span>|<span data-ttu-id="0faa7-175">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-175">String</span></span>|<span data-ttu-id="0faa7-176">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="0faa7-176">The developer of the app.</span></span> <span data-ttu-id="0faa7-177">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-178">notes</span><span class="sxs-lookup"><span data-stu-id="0faa7-178">notes</span></span>|<span data-ttu-id="0faa7-179">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-179">String</span></span>|<span data-ttu-id="0faa7-180">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="0faa7-180">Notes for the app.</span></span> <span data-ttu-id="0faa7-181">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0faa7-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="0faa7-182">publishingState</span></span>|[<span data-ttu-id="0faa7-183">Мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="0faa7-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0faa7-184">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="0faa7-184">The publishing state for the app.</span></span> <span data-ttu-id="0faa7-185">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="0faa7-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0faa7-186">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0faa7-187">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="0faa7-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0faa7-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="0faa7-188">committedContentVersion</span></span>|<span data-ttu-id="0faa7-189">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-189">String</span></span>|<span data-ttu-id="0faa7-190">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="0faa7-190">The internal committed content version.</span></span> <span data-ttu-id="0faa7-191">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0faa7-192">fileName</span><span class="sxs-lookup"><span data-stu-id="0faa7-192">fileName</span></span>|<span data-ttu-id="0faa7-193">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-193">String</span></span>|<span data-ttu-id="0faa7-194">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="0faa7-194">The name of the main Lob application file.</span></span> <span data-ttu-id="0faa7-195">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0faa7-196">size</span><span class="sxs-lookup"><span data-stu-id="0faa7-196">size</span></span>|<span data-ttu-id="0faa7-197">Int64</span><span class="sxs-lookup"><span data-stu-id="0faa7-197">Int64</span></span>|<span data-ttu-id="0faa7-198">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="0faa7-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="0faa7-199">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="0faa7-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="0faa7-200">packageId</span><span class="sxs-lookup"><span data-stu-id="0faa7-200">packageId</span></span>|<span data-ttu-id="0faa7-201">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-201">String</span></span>|<span data-ttu-id="0faa7-202">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="0faa7-202">The package identifier.</span></span>|
|<span data-ttu-id="0faa7-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0faa7-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0faa7-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0faa7-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="0faa7-205">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="0faa7-205">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="0faa7-206">versionName</span><span class="sxs-lookup"><span data-stu-id="0faa7-206">versionName</span></span>|<span data-ttu-id="0faa7-207">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-207">String</span></span>|<span data-ttu-id="0faa7-208">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="0faa7-208">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0faa7-209">versionCode</span><span class="sxs-lookup"><span data-stu-id="0faa7-209">versionCode</span></span>|<span data-ttu-id="0faa7-210">String</span><span class="sxs-lookup"><span data-stu-id="0faa7-210">String</span></span>|<span data-ttu-id="0faa7-211">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="0faa7-211">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="0faa7-212">Ответ</span><span class="sxs-lookup"><span data-stu-id="0faa7-212">Response</span></span>
<span data-ttu-id="0faa7-213">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0faa7-213">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0faa7-214">Пример</span><span class="sxs-lookup"><span data-stu-id="0faa7-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="0faa7-215">Запрос</span><span class="sxs-lookup"><span data-stu-id="0faa7-215">Request</span></span>
<span data-ttu-id="0faa7-216">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0faa7-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0faa7-217">Отклик</span><span class="sxs-lookup"><span data-stu-id="0faa7-217">Response</span></span>
<span data-ttu-id="0faa7-p118">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0faa7-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



