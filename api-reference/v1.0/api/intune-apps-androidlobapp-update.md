---
title: Update androidLobApp
description: Обновление свойств объекта androidLobApp.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca5c8b1242e5805b00150ebfc79ba0d88499d241
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42516667"
---
# <a name="update-androidlobapp"></a><span data-ttu-id="d97a9-103">Update androidLobApp</span><span class="sxs-lookup"><span data-stu-id="d97a9-103">Update androidLobApp</span></span>

<span data-ttu-id="d97a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d97a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d97a9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d97a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d97a9-106">Обновление свойств объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-106">Update the properties of a [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d97a9-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d97a9-107">Prerequisites</span></span>
<span data-ttu-id="d97a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d97a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d97a9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d97a9-110">Permission type</span></span>|<span data-ttu-id="d97a9-111">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="d97a9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d97a9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d97a9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d97a9-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d97a9-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d97a9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d97a9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d97a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d97a9-115">Not supported.</span></span>|
|<span data-ttu-id="d97a9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d97a9-116">Application</span></span>|<span data-ttu-id="d97a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d97a9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d97a9-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d97a9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d97a9-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d97a9-119">Request headers</span></span>
|<span data-ttu-id="d97a9-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d97a9-120">Header</span></span>|<span data-ttu-id="d97a9-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d97a9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d97a9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d97a9-122">Authorization</span></span>|<span data-ttu-id="d97a9-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d97a9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d97a9-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d97a9-124">Accept</span></span>|<span data-ttu-id="d97a9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d97a9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d97a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d97a9-126">Request body</span></span>
<span data-ttu-id="d97a9-127">В теле запроса добавьте представление объекта [androidLobApp](../resources/intune-apps-androidlobapp.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d97a9-127">In the request body, supply a JSON representation for the [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

<span data-ttu-id="d97a9-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-128">The following table shows the properties that are required when you create the [androidLobApp](../resources/intune-apps-androidlobapp.md).</span></span>

|<span data-ttu-id="d97a9-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d97a9-129">Property</span></span>|<span data-ttu-id="d97a9-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d97a9-130">Type</span></span>|<span data-ttu-id="d97a9-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d97a9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d97a9-132">id</span><span class="sxs-lookup"><span data-stu-id="d97a9-132">id</span></span>|<span data-ttu-id="d97a9-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-133">String</span></span>|<span data-ttu-id="d97a9-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d97a9-134">Key of the entity.</span></span> <span data-ttu-id="d97a9-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d97a9-136">displayName</span></span>|<span data-ttu-id="d97a9-137">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-137">String</span></span>|<span data-ttu-id="d97a9-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d97a9-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d97a9-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-140">description</span><span class="sxs-lookup"><span data-stu-id="d97a9-140">description</span></span>|<span data-ttu-id="d97a9-141">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-141">String</span></span>|<span data-ttu-id="d97a9-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d97a9-142">The description of the app.</span></span> <span data-ttu-id="d97a9-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-144">publisher</span><span class="sxs-lookup"><span data-stu-id="d97a9-144">publisher</span></span>|<span data-ttu-id="d97a9-145">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-145">String</span></span>|<span data-ttu-id="d97a9-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d97a9-146">The publisher of the app.</span></span> <span data-ttu-id="d97a9-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d97a9-148">largeIcon</span></span>|[<span data-ttu-id="d97a9-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d97a9-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d97a9-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d97a9-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d97a9-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d97a9-152">createdDateTime</span></span>|<span data-ttu-id="d97a9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d97a9-153">DateTimeOffset</span></span>|<span data-ttu-id="d97a9-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d97a9-154">The date and time the app was created.</span></span> <span data-ttu-id="d97a9-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d97a9-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d97a9-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d97a9-157">DateTimeOffset</span></span>|<span data-ttu-id="d97a9-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d97a9-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d97a9-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d97a9-160">isFeatured</span></span>|<span data-ttu-id="d97a9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d97a9-161">Boolean</span></span>|<span data-ttu-id="d97a9-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d97a9-163">privacyInformationUrl</span></span>|<span data-ttu-id="d97a9-164">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-164">String</span></span>|<span data-ttu-id="d97a9-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d97a9-165">The privacy statement Url.</span></span> <span data-ttu-id="d97a9-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d97a9-167">informationUrl</span></span>|<span data-ttu-id="d97a9-168">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-168">String</span></span>|<span data-ttu-id="d97a9-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d97a9-169">The more information Url.</span></span> <span data-ttu-id="d97a9-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-171">owner</span><span class="sxs-lookup"><span data-stu-id="d97a9-171">owner</span></span>|<span data-ttu-id="d97a9-172">String</span><span class="sxs-lookup"><span data-stu-id="d97a9-172">String</span></span>|<span data-ttu-id="d97a9-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d97a9-173">The owner of the app.</span></span> <span data-ttu-id="d97a9-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-175">developer</span><span class="sxs-lookup"><span data-stu-id="d97a9-175">developer</span></span>|<span data-ttu-id="d97a9-176">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-176">String</span></span>|<span data-ttu-id="d97a9-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d97a9-177">The developer of the app.</span></span> <span data-ttu-id="d97a9-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-179">notes</span><span class="sxs-lookup"><span data-stu-id="d97a9-179">notes</span></span>|<span data-ttu-id="d97a9-180">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-180">String</span></span>|<span data-ttu-id="d97a9-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d97a9-181">Notes for the app.</span></span> <span data-ttu-id="d97a9-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d97a9-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="d97a9-183">publishingState</span></span>|[<span data-ttu-id="d97a9-184">мобилеапппублишингстате</span><span class="sxs-lookup"><span data-stu-id="d97a9-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d97a9-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d97a9-185">The publishing state for the app.</span></span> <span data-ttu-id="d97a9-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d97a9-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d97a9-187">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d97a9-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d97a9-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d97a9-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d97a9-189">committedContentVersion</span></span>|<span data-ttu-id="d97a9-190">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-190">String</span></span>|<span data-ttu-id="d97a9-191">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="d97a9-191">The internal committed content version.</span></span> <span data-ttu-id="d97a9-192">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d97a9-193">fileName</span><span class="sxs-lookup"><span data-stu-id="d97a9-193">fileName</span></span>|<span data-ttu-id="d97a9-194">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-194">String</span></span>|<span data-ttu-id="d97a9-195">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="d97a9-195">The name of the main Lob application file.</span></span> <span data-ttu-id="d97a9-196">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d97a9-197">size</span><span class="sxs-lookup"><span data-stu-id="d97a9-197">size</span></span>|<span data-ttu-id="d97a9-198">Int64</span><span class="sxs-lookup"><span data-stu-id="d97a9-198">Int64</span></span>|<span data-ttu-id="d97a9-199">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="d97a9-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="d97a9-200">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d97a9-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d97a9-201">packageId</span><span class="sxs-lookup"><span data-stu-id="d97a9-201">packageId</span></span>|<span data-ttu-id="d97a9-202">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-202">String</span></span>|<span data-ttu-id="d97a9-203">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="d97a9-203">The package identifier.</span></span>|
|<span data-ttu-id="d97a9-204">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d97a9-204">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d97a9-205">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d97a9-205">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="d97a9-206">Значение, которое представляет минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="d97a9-206">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d97a9-207">versionName</span><span class="sxs-lookup"><span data-stu-id="d97a9-207">versionName</span></span>|<span data-ttu-id="d97a9-208">Строка</span><span class="sxs-lookup"><span data-stu-id="d97a9-208">String</span></span>|<span data-ttu-id="d97a9-209">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="d97a9-209">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d97a9-210">versionCode</span><span class="sxs-lookup"><span data-stu-id="d97a9-210">versionCode</span></span>|<span data-ttu-id="d97a9-211">String</span><span class="sxs-lookup"><span data-stu-id="d97a9-211">String</span></span>|<span data-ttu-id="d97a9-212">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="d97a9-212">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="d97a9-213">Ответ</span><span class="sxs-lookup"><span data-stu-id="d97a9-213">Response</span></span>
<span data-ttu-id="d97a9-214">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d97a9-214">If successful, this method returns a `200 OK` response code and an updated [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d97a9-215">Пример</span><span class="sxs-lookup"><span data-stu-id="d97a9-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="d97a9-216">Запрос</span><span class="sxs-lookup"><span data-stu-id="d97a9-216">Request</span></span>
<span data-ttu-id="d97a9-217">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d97a9-217">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="d97a9-218">Отклик</span><span class="sxs-lookup"><span data-stu-id="d97a9-218">Response</span></span>
<span data-ttu-id="d97a9-p118">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d97a9-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




