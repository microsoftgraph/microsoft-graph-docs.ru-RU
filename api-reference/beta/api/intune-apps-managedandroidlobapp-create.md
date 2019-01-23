---
title: Create managedAndroidLobApp
description: Создание объекта managedAndroidLobApp.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: deeb2b1810d56f8b0d704476149af90bc2248927
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398081"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="c7155-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="c7155-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="c7155-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c7155-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c7155-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7155-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7155-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c7155-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7155-107">Создание объекта [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-107">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7155-108">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="c7155-108">Prerequisites</span></span>
<span data-ttu-id="c7155-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c7155-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7155-111">Permission type</span></span>|<span data-ttu-id="c7155-112">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7155-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7155-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7155-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7155-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7155-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c7155-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7155-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7155-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7155-116">Not supported.</span></span>|
|<span data-ttu-id="c7155-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7155-117">Application</span></span>|<span data-ttu-id="c7155-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c7155-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7155-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7155-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c7155-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7155-120">Request headers</span></span>
|<span data-ttu-id="c7155-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c7155-121">Header</span></span>|<span data-ttu-id="c7155-122">Значение</span><span class="sxs-lookup"><span data-stu-id="c7155-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7155-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7155-123">Authorization</span></span>|<span data-ttu-id="c7155-124">Требуется Bearer &lt;маркер&gt;
</span><span class="sxs-lookup"><span data-stu-id="c7155-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7155-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c7155-125">Accept</span></span>|<span data-ttu-id="c7155-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c7155-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7155-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7155-127">Request body</span></span>
<span data-ttu-id="c7155-128">В тексте запроса добавьте представление объекта managedAndroidLobApp в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c7155-128">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="c7155-129">В приведенной ниже таблице показаны свойства, которые необходимо указывать при создании объекта managedAndroidLobApp.</span><span class="sxs-lookup"><span data-stu-id="c7155-129">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="c7155-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="c7155-130">Property</span></span>|<span data-ttu-id="c7155-131">Тип</span><span class="sxs-lookup"><span data-stu-id="c7155-131">Type</span></span>|<span data-ttu-id="c7155-132">Описание</span><span class="sxs-lookup"><span data-stu-id="c7155-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7155-133">id</span><span class="sxs-lookup"><span data-stu-id="c7155-133">id</span></span>|<span data-ttu-id="c7155-134">String</span><span class="sxs-lookup"><span data-stu-id="c7155-134">String</span></span>|<span data-ttu-id="c7155-135">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="c7155-135">Key of the entity.</span></span> <span data-ttu-id="c7155-136">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c7155-137">displayName</span></span>|<span data-ttu-id="c7155-138">String</span><span class="sxs-lookup"><span data-stu-id="c7155-138">String</span></span>|<span data-ttu-id="c7155-139">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="c7155-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c7155-140">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-141">description</span><span class="sxs-lookup"><span data-stu-id="c7155-141">description</span></span>|<span data-ttu-id="c7155-142">String</span><span class="sxs-lookup"><span data-stu-id="c7155-142">String</span></span>|<span data-ttu-id="c7155-143">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-143">The description of the app.</span></span> <span data-ttu-id="c7155-144">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c7155-145">publisher</span></span>|<span data-ttu-id="c7155-146">String</span><span class="sxs-lookup"><span data-stu-id="c7155-146">String</span></span>|<span data-ttu-id="c7155-147">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-147">The publisher of the app.</span></span> <span data-ttu-id="c7155-148">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c7155-149">largeIcon</span></span>|[<span data-ttu-id="c7155-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c7155-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c7155-151">Большой значок, который отображается в сведениях о приложении и используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="c7155-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c7155-152">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c7155-153">createdDateTime</span></span>|<span data-ttu-id="c7155-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7155-154">DateTimeOffset</span></span>|<span data-ttu-id="c7155-155">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-155">The date and time the app was created.</span></span> <span data-ttu-id="c7155-156">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c7155-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c7155-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7155-158">DateTimeOffset</span></span>|<span data-ttu-id="c7155-159">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c7155-160">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c7155-161">isFeatured</span></span>|<span data-ttu-id="c7155-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c7155-162">Boolean</span></span>|<span data-ttu-id="c7155-163">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c7155-164">privacyInformationUrl</span></span>|<span data-ttu-id="c7155-165">String</span><span class="sxs-lookup"><span data-stu-id="c7155-165">String</span></span>|<span data-ttu-id="c7155-166">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="c7155-166">The privacy statement Url.</span></span> <span data-ttu-id="c7155-167">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c7155-168">informationUrl</span></span>|<span data-ttu-id="c7155-169">String</span><span class="sxs-lookup"><span data-stu-id="c7155-169">String</span></span>|<span data-ttu-id="c7155-170">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="c7155-170">The more information Url.</span></span> <span data-ttu-id="c7155-171">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-172">owner</span><span class="sxs-lookup"><span data-stu-id="c7155-172">owner</span></span>|<span data-ttu-id="c7155-173">String</span><span class="sxs-lookup"><span data-stu-id="c7155-173">String</span></span>|<span data-ttu-id="c7155-174">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-174">The owner of the app.</span></span> <span data-ttu-id="c7155-175">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-176">developer</span><span class="sxs-lookup"><span data-stu-id="c7155-176">developer</span></span>|<span data-ttu-id="c7155-177">String</span><span class="sxs-lookup"><span data-stu-id="c7155-177">String</span></span>|<span data-ttu-id="c7155-178">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-178">The developer of the app.</span></span> <span data-ttu-id="c7155-179">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-180">notes</span><span class="sxs-lookup"><span data-stu-id="c7155-180">notes</span></span>|<span data-ttu-id="c7155-181">String</span><span class="sxs-lookup"><span data-stu-id="c7155-181">String</span></span>|<span data-ttu-id="c7155-182">Примечания к приложению.</span><span class="sxs-lookup"><span data-stu-id="c7155-182">Notes for the app.</span></span> <span data-ttu-id="c7155-183">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c7155-184">uploadState</span></span>|<span data-ttu-id="c7155-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c7155-185">Int32</span></span>|<span data-ttu-id="c7155-186">Состояние передачи.</span><span class="sxs-lookup"><span data-stu-id="c7155-186">The upload state.</span></span> <span data-ttu-id="c7155-187">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c7155-188">publishingState</span></span>|[<span data-ttu-id="c7155-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c7155-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c7155-190">Состояние публикации приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-190">The publishing state for the app.</span></span> <span data-ttu-id="c7155-191">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="c7155-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c7155-192">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c7155-193">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="c7155-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c7155-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c7155-194">isAssigned</span></span>|<span data-ttu-id="c7155-195">Логический</span><span class="sxs-lookup"><span data-stu-id="c7155-195">Boolean</span></span>|<span data-ttu-id="c7155-196">Значение, указывающее, назначена ли приложение по крайней мере одной группы.</span><span class="sxs-lookup"><span data-stu-id="c7155-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c7155-197">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c7155-198">roleScopeTagIds</span></span>|<span data-ttu-id="c7155-199">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="c7155-199">String collection</span></span>|<span data-ttu-id="c7155-200">Список идентификаторов тег области для данного мобильного приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c7155-201">Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c7155-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="c7155-202">appAvailability</span></span>|[<span data-ttu-id="c7155-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="c7155-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="c7155-204">Доступность приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-204">The Application's availability.</span></span> <span data-ttu-id="c7155-205">Наследуется от [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="c7155-206">Возможные значения: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="c7155-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="c7155-207">version</span><span class="sxs-lookup"><span data-stu-id="c7155-207">version</span></span>|<span data-ttu-id="c7155-208">String</span><span class="sxs-lookup"><span data-stu-id="c7155-208">String</span></span>|<span data-ttu-id="c7155-209">Версия приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-209">The Application's version.</span></span> <span data-ttu-id="c7155-210">Наследуется от объекта [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="c7155-211">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c7155-211">committedContentVersion</span></span>|<span data-ttu-id="c7155-212">String</span><span class="sxs-lookup"><span data-stu-id="c7155-212">String</span></span>|<span data-ttu-id="c7155-213">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="c7155-213">The internal committed content version.</span></span> <span data-ttu-id="c7155-214">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="c7155-215">fileName</span><span class="sxs-lookup"><span data-stu-id="c7155-215">fileName</span></span>|<span data-ttu-id="c7155-216">String</span><span class="sxs-lookup"><span data-stu-id="c7155-216">String</span></span>|<span data-ttu-id="c7155-217">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="c7155-217">The name of the main Lob application file.</span></span> <span data-ttu-id="c7155-218">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="c7155-219">size</span><span class="sxs-lookup"><span data-stu-id="c7155-219">size</span></span>|<span data-ttu-id="c7155-220">Int64</span><span class="sxs-lookup"><span data-stu-id="c7155-220">Int64</span></span>|<span data-ttu-id="c7155-221">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="c7155-221">The total size, including all uploaded files.</span></span> <span data-ttu-id="c7155-222">Наследуется от объекта [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="c7155-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="c7155-223">packageId</span><span class="sxs-lookup"><span data-stu-id="c7155-223">packageId</span></span>|<span data-ttu-id="c7155-224">String</span><span class="sxs-lookup"><span data-stu-id="c7155-224">String</span></span>|<span data-ttu-id="c7155-225">Идентификатор пакета.</span><span class="sxs-lookup"><span data-stu-id="c7155-225">The package identifier.</span></span>|
|<span data-ttu-id="c7155-226">identityName</span><span class="sxs-lookup"><span data-stu-id="c7155-226">identityName</span></span>|<span data-ttu-id="c7155-227">String</span><span class="sxs-lookup"><span data-stu-id="c7155-227">String</span></span>|<span data-ttu-id="c7155-228">Имя удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c7155-228">The Identity Name.</span></span>|
|<span data-ttu-id="c7155-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c7155-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="c7155-230">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="c7155-230">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="c7155-231">Значение, указывающее минимальную применимую версию операционной системы.</span><span class="sxs-lookup"><span data-stu-id="c7155-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="c7155-232">versionName</span><span class="sxs-lookup"><span data-stu-id="c7155-232">versionName</span></span>|<span data-ttu-id="c7155-233">String</span><span class="sxs-lookup"><span data-stu-id="c7155-233">String</span></span>|<span data-ttu-id="c7155-234">Имя версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="c7155-234">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c7155-235">versionCode</span><span class="sxs-lookup"><span data-stu-id="c7155-235">versionCode</span></span>|<span data-ttu-id="c7155-236">String</span><span class="sxs-lookup"><span data-stu-id="c7155-236">String</span></span>|<span data-ttu-id="c7155-237">Код версии управляемого бизнес-приложения для Android.</span><span class="sxs-lookup"><span data-stu-id="c7155-237">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="c7155-238">identityVersion</span><span class="sxs-lookup"><span data-stu-id="c7155-238">identityVersion</span></span>|<span data-ttu-id="c7155-239">String</span><span class="sxs-lookup"><span data-stu-id="c7155-239">String</span></span>|<span data-ttu-id="c7155-240">Версия удостоверения.</span><span class="sxs-lookup"><span data-stu-id="c7155-240">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="c7155-241">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7155-241">Response</span></span>
<span data-ttu-id="c7155-242">В случае успешного выполнения этот метод возвращает код ответа `201 Created` и объект [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c7155-242">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7155-243">Пример</span><span class="sxs-lookup"><span data-stu-id="c7155-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7155-244">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7155-244">Request</span></span>
<span data-ttu-id="c7155-245">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7155-245">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1464

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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

### <a name="response"></a><span data-ttu-id="c7155-246">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7155-246">Response</span></span>
<span data-ttu-id="c7155-p124">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="c7155-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1636

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
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




