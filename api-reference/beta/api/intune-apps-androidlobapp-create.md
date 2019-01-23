---
title: Create androidLobApp
description: Создание нового объекта androidLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4d08ae1af5c5415c22c70d45e3d7a0c264e3069f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399236"
---
# <a name="create-androidlobapp"></a><span data-ttu-id="3c376-103">Create androidLobApp</span><span class="sxs-lookup"><span data-stu-id="3c376-103">Create androidLobApp</span></span>

> <span data-ttu-id="3c376-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3c376-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3c376-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c376-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3c376-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c376-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c376-107">Создание нового объекта [androidLobApp](../resources/intune-apps-androidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-107">Create a new [androidLobApp](../resources/intune-apps-androidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c376-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="3c376-108">Prerequisites</span></span>
<span data-ttu-id="3c376-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3c376-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3c376-111">Permission type</span></span>|<span data-ttu-id="3c376-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3c376-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c376-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3c376-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c376-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c376-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c376-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3c376-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c376-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c376-116">Not supported.</span></span>|
|<span data-ttu-id="3c376-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3c376-117">Application</span></span>|<span data-ttu-id="3c376-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3c376-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c376-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3c376-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3c376-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3c376-120">Request headers</span></span>
|<span data-ttu-id="3c376-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3c376-121">Header</span></span>|<span data-ttu-id="3c376-122">Значение</span><span class="sxs-lookup"><span data-stu-id="3c376-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c376-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c376-123">Authorization</span></span>|<span data-ttu-id="3c376-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="3c376-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c376-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3c376-125">Accept</span></span>|<span data-ttu-id="3c376-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c376-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c376-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="3c376-127">Request body</span></span>
<span data-ttu-id="3c376-128">В теле запроса добавьте представление объекта androidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c376-128">In the request body, supply a JSON representation for the androidLobApp object.</span></span>

<span data-ttu-id="3c376-129">Ниже показаны свойства, которые необходимо указывать при создании объекта androidLobApp.</span><span class="sxs-lookup"><span data-stu-id="3c376-129">The following table shows the properties that are required when you create the androidLobApp.</span></span>

|<span data-ttu-id="3c376-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c376-130">Property</span></span>|<span data-ttu-id="3c376-131">Тип</span><span class="sxs-lookup"><span data-stu-id="3c376-131">Type</span></span>|<span data-ttu-id="3c376-132">Описание</span><span class="sxs-lookup"><span data-stu-id="3c376-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c376-133">id</span><span class="sxs-lookup"><span data-stu-id="3c376-133">id</span></span>|<span data-ttu-id="3c376-134">String</span><span class="sxs-lookup"><span data-stu-id="3c376-134">String</span></span>|<span data-ttu-id="3c376-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="3c376-135">Key of the entity.</span></span> <span data-ttu-id="3c376-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3c376-137">displayName</span></span>|<span data-ttu-id="3c376-138">String</span><span class="sxs-lookup"><span data-stu-id="3c376-138">String</span></span>|<span data-ttu-id="3c376-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="3c376-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3c376-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-141">description</span><span class="sxs-lookup"><span data-stu-id="3c376-141">description</span></span>|<span data-ttu-id="3c376-142">String</span><span class="sxs-lookup"><span data-stu-id="3c376-142">String</span></span>|<span data-ttu-id="3c376-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="3c376-143">The description of the app.</span></span> <span data-ttu-id="3c376-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-145">publisher</span><span class="sxs-lookup"><span data-stu-id="3c376-145">publisher</span></span>|<span data-ttu-id="3c376-146">String</span><span class="sxs-lookup"><span data-stu-id="3c376-146">String</span></span>|<span data-ttu-id="3c376-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="3c376-147">The publisher of the app.</span></span> <span data-ttu-id="3c376-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3c376-149">largeIcon</span></span>|[<span data-ttu-id="3c376-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3c376-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3c376-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="3c376-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3c376-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c376-153">createdDateTime</span></span>|<span data-ttu-id="3c376-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c376-154">DateTimeOffset</span></span>|<span data-ttu-id="3c376-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="3c376-155">The date and time the app was created.</span></span> <span data-ttu-id="3c376-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c376-157">lastModifiedDateTime</span></span>|<span data-ttu-id="3c376-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c376-158">DateTimeOffset</span></span>|<span data-ttu-id="3c376-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="3c376-159">The date and time the app was last modified.</span></span> <span data-ttu-id="3c376-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3c376-161">isFeatured</span></span>|<span data-ttu-id="3c376-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c376-162">Boolean</span></span>|<span data-ttu-id="3c376-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3c376-164">privacyInformationUrl</span></span>|<span data-ttu-id="3c376-165">String</span><span class="sxs-lookup"><span data-stu-id="3c376-165">String</span></span>|<span data-ttu-id="3c376-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="3c376-166">The privacy statement Url.</span></span> <span data-ttu-id="3c376-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3c376-168">informationUrl</span></span>|<span data-ttu-id="3c376-169">String</span><span class="sxs-lookup"><span data-stu-id="3c376-169">String</span></span>|<span data-ttu-id="3c376-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="3c376-170">The more information Url.</span></span> <span data-ttu-id="3c376-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-172">owner</span><span class="sxs-lookup"><span data-stu-id="3c376-172">owner</span></span>|<span data-ttu-id="3c376-173">String</span><span class="sxs-lookup"><span data-stu-id="3c376-173">String</span></span>|<span data-ttu-id="3c376-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="3c376-174">The owner of the app.</span></span> <span data-ttu-id="3c376-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-176">developer</span><span class="sxs-lookup"><span data-stu-id="3c376-176">developer</span></span>|<span data-ttu-id="3c376-177">String</span><span class="sxs-lookup"><span data-stu-id="3c376-177">String</span></span>|<span data-ttu-id="3c376-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="3c376-178">The developer of the app.</span></span> <span data-ttu-id="3c376-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-180">notes</span><span class="sxs-lookup"><span data-stu-id="3c376-180">notes</span></span>|<span data-ttu-id="3c376-181">String</span><span class="sxs-lookup"><span data-stu-id="3c376-181">String</span></span>|<span data-ttu-id="3c376-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="3c376-182">Notes for the app.</span></span> <span data-ttu-id="3c376-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="3c376-184">uploadState</span></span>|<span data-ttu-id="3c376-185">Int32</span><span class="sxs-lookup"><span data-stu-id="3c376-185">Int32</span></span>|<span data-ttu-id="3c376-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="3c376-186">The upload state.</span></span> <span data-ttu-id="3c376-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="3c376-188">publishingState</span></span>|[<span data-ttu-id="3c376-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3c376-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3c376-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="3c376-190">The publishing state for the app.</span></span> <span data-ttu-id="3c376-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="3c376-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3c376-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3c376-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3c376-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3c376-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="3c376-194">isAssigned</span></span>|<span data-ttu-id="3c376-195">Логический</span><span class="sxs-lookup"><span data-stu-id="3c376-195">Boolean</span></span>|<span data-ttu-id="3c376-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="3c376-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="3c376-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3c376-198">roleScopeTagIds</span></span>|<span data-ttu-id="3c376-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3c376-199">String collection</span></span>|<span data-ttu-id="3c376-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="3c376-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="3c376-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3c376-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3c376-202">committedContentVersion</span></span>|<span data-ttu-id="3c376-203">String</span><span class="sxs-lookup"><span data-stu-id="3c376-203">String</span></span>|<span data-ttu-id="3c376-204">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="3c376-204">The internal committed content version.</span></span> <span data-ttu-id="3c376-205">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3c376-206">fileName</span><span class="sxs-lookup"><span data-stu-id="3c376-206">fileName</span></span>|<span data-ttu-id="3c376-207">String</span><span class="sxs-lookup"><span data-stu-id="3c376-207">String</span></span>|<span data-ttu-id="3c376-208">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="3c376-208">The name of the main Lob application file.</span></span> <span data-ttu-id="3c376-209">Наследуется от объекта [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3c376-210">size</span><span class="sxs-lookup"><span data-stu-id="3c376-210">size</span></span>|<span data-ttu-id="3c376-211">Int64</span><span class="sxs-lookup"><span data-stu-id="3c376-211">Int64</span></span>|<span data-ttu-id="3c376-212">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="3c376-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="3c376-213">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3c376-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="3c376-214">packageId</span><span class="sxs-lookup"><span data-stu-id="3c376-214">packageId</span></span>|<span data-ttu-id="3c376-215">String</span><span class="sxs-lookup"><span data-stu-id="3c376-215">String</span></span>|<span data-ttu-id="3c376-216">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="3c376-216">The package identifier.</span></span>|
|<span data-ttu-id="3c376-217">identityName</span><span class="sxs-lookup"><span data-stu-id="3c376-217">identityName</span></span>|<span data-ttu-id="3c376-218">String</span><span class="sxs-lookup"><span data-stu-id="3c376-218">String</span></span>|<span data-ttu-id="3c376-219">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3c376-219">The Identity Name.</span></span>|
|<span data-ttu-id="3c376-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3c376-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3c376-221">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3c376-221">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="3c376-222">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="3c376-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3c376-223">versionName</span><span class="sxs-lookup"><span data-stu-id="3c376-223">versionName</span></span>|<span data-ttu-id="3c376-224">String</span><span class="sxs-lookup"><span data-stu-id="3c376-224">String</span></span>|<span data-ttu-id="3c376-225">Имя версии бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="3c376-225">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3c376-226">versionCode</span><span class="sxs-lookup"><span data-stu-id="3c376-226">versionCode</span></span>|<span data-ttu-id="3c376-227">String</span><span class="sxs-lookup"><span data-stu-id="3c376-227">String</span></span>|<span data-ttu-id="3c376-228">Код версии бизнес-приложения Android.</span><span class="sxs-lookup"><span data-stu-id="3c376-228">The version code of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3c376-229">identityVersion</span><span class="sxs-lookup"><span data-stu-id="3c376-229">identityVersion</span></span>|<span data-ttu-id="3c376-230">String</span><span class="sxs-lookup"><span data-stu-id="3c376-230">String</span></span>|<span data-ttu-id="3c376-231">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3c376-231">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="3c376-232">Ответ</span><span class="sxs-lookup"><span data-stu-id="3c376-232">Response</span></span>
<span data-ttu-id="3c376-233">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [androidLobApp](../resources/intune-apps-androidlobapp.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="3c376-233">If successful, this method returns a `201 Created` response code and a [androidLobApp](../resources/intune-apps-androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c376-234">Пример</span><span class="sxs-lookup"><span data-stu-id="3c376-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c376-235">Запрос</span><span class="sxs-lookup"><span data-stu-id="3c376-235">Request</span></span>
<span data-ttu-id="3c376-236">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3c376-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1386

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="3c376-237">Отклик</span><span class="sxs-lookup"><span data-stu-id="3c376-237">Response</span></span>
<span data-ttu-id="3c376-p122">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="3c376-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1558

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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
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
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```




