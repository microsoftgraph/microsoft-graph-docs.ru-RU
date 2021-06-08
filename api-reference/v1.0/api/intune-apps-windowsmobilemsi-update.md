---
title: Update windowsMobileMSI
description: Обновление свойств объекта windowsMobileMSI.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2a8451e594816953c76c9e4f24c53b486af2b49f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759653"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="d7280-103">Update windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="d7280-103">Update windowsMobileMSI</span></span>

<span data-ttu-id="d7280-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7280-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d7280-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d7280-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7280-106">Обновление свойств объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-106">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d7280-107">Необходимые разрешения</span><span class="sxs-lookup"><span data-stu-id="d7280-107">Prerequisites</span></span>
<span data-ttu-id="d7280-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7280-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7280-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7280-110">Permission type</span></span>|<span data-ttu-id="d7280-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7280-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7280-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7280-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7280-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7280-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d7280-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7280-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7280-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7280-115">Not supported.</span></span>|
|<span data-ttu-id="d7280-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d7280-116">Application</span></span>|<span data-ttu-id="d7280-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7280-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7280-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7280-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d7280-119">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="d7280-119">Request headers</span></span>
|<span data-ttu-id="d7280-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7280-120">Header</span></span>|<span data-ttu-id="d7280-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d7280-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7280-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7280-122">Authorization</span></span>|<span data-ttu-id="d7280-123">Bearer &lt;token&gt;. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7280-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7280-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d7280-124">Accept</span></span>|<span data-ttu-id="d7280-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d7280-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7280-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7280-126">Request body</span></span>
<span data-ttu-id="d7280-127">В теле запроса добавьте представление объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7280-127">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="d7280-128">Ниже показаны свойства, которые необходимо указывать при создании объекта [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-128">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="d7280-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7280-129">Property</span></span>|<span data-ttu-id="d7280-130">Тип</span><span class="sxs-lookup"><span data-stu-id="d7280-130">Type</span></span>|<span data-ttu-id="d7280-131">Описание</span><span class="sxs-lookup"><span data-stu-id="d7280-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7280-132">id</span><span class="sxs-lookup"><span data-stu-id="d7280-132">id</span></span>|<span data-ttu-id="d7280-133">String</span><span class="sxs-lookup"><span data-stu-id="d7280-133">String</span></span>|<span data-ttu-id="d7280-134">Ключ объекта.</span><span class="sxs-lookup"><span data-stu-id="d7280-134">Key of the entity.</span></span> <span data-ttu-id="d7280-135">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-136">displayName</span><span class="sxs-lookup"><span data-stu-id="d7280-136">displayName</span></span>|<span data-ttu-id="d7280-137">String</span><span class="sxs-lookup"><span data-stu-id="d7280-137">String</span></span>|<span data-ttu-id="d7280-138">Название приложения, которое предоставил или импортировал администратор.</span><span class="sxs-lookup"><span data-stu-id="d7280-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d7280-139">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-140">description</span><span class="sxs-lookup"><span data-stu-id="d7280-140">description</span></span>|<span data-ttu-id="d7280-141">String</span><span class="sxs-lookup"><span data-stu-id="d7280-141">String</span></span>|<span data-ttu-id="d7280-142">Описание приложения.</span><span class="sxs-lookup"><span data-stu-id="d7280-142">The description of the app.</span></span> <span data-ttu-id="d7280-143">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-144">publisher</span><span class="sxs-lookup"><span data-stu-id="d7280-144">publisher</span></span>|<span data-ttu-id="d7280-145">String</span><span class="sxs-lookup"><span data-stu-id="d7280-145">String</span></span>|<span data-ttu-id="d7280-146">Издатель приложения.</span><span class="sxs-lookup"><span data-stu-id="d7280-146">The publisher of the app.</span></span> <span data-ttu-id="d7280-147">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d7280-148">largeIcon</span></span>|[<span data-ttu-id="d7280-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d7280-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d7280-150">Представляет большой значок, который отображается в сведениях о приложении, используется для отправки значка.</span><span class="sxs-lookup"><span data-stu-id="d7280-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d7280-151">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d7280-152">createdDateTime</span></span>|<span data-ttu-id="d7280-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7280-153">DateTimeOffset</span></span>|<span data-ttu-id="d7280-154">Дата и время создания приложения.</span><span class="sxs-lookup"><span data-stu-id="d7280-154">The date and time the app was created.</span></span> <span data-ttu-id="d7280-155">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d7280-156">lastModifiedDateTime</span></span>|<span data-ttu-id="d7280-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7280-157">DateTimeOffset</span></span>|<span data-ttu-id="d7280-158">Дата и время последнего изменения приложения.</span><span class="sxs-lookup"><span data-stu-id="d7280-158">The date and time the app was last modified.</span></span> <span data-ttu-id="d7280-159">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d7280-160">isFeatured</span></span>|<span data-ttu-id="d7280-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7280-161">Boolean</span></span>|<span data-ttu-id="d7280-162">Значение, которое показывает, отмечено ли приложение как подобранное администратором. Наследуется от объекта [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d7280-163">privacyInformationUrl</span></span>|<span data-ttu-id="d7280-164">String</span><span class="sxs-lookup"><span data-stu-id="d7280-164">String</span></span>|<span data-ttu-id="d7280-165">URL-адрес заявления о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="d7280-165">The privacy statement Url.</span></span> <span data-ttu-id="d7280-166">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d7280-167">informationUrl</span></span>|<span data-ttu-id="d7280-168">String</span><span class="sxs-lookup"><span data-stu-id="d7280-168">String</span></span>|<span data-ttu-id="d7280-169">URL-адрес страницы с дополнительными сведениями.</span><span class="sxs-lookup"><span data-stu-id="d7280-169">The more information Url.</span></span> <span data-ttu-id="d7280-170">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-171">owner</span><span class="sxs-lookup"><span data-stu-id="d7280-171">owner</span></span>|<span data-ttu-id="d7280-172">String</span><span class="sxs-lookup"><span data-stu-id="d7280-172">String</span></span>|<span data-ttu-id="d7280-173">Владелец приложения.</span><span class="sxs-lookup"><span data-stu-id="d7280-173">The owner of the app.</span></span> <span data-ttu-id="d7280-174">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-175">developer</span><span class="sxs-lookup"><span data-stu-id="d7280-175">developer</span></span>|<span data-ttu-id="d7280-176">String</span><span class="sxs-lookup"><span data-stu-id="d7280-176">String</span></span>|<span data-ttu-id="d7280-177">Разработчик приложения.</span><span class="sxs-lookup"><span data-stu-id="d7280-177">The developer of the app.</span></span> <span data-ttu-id="d7280-178">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-179">notes</span><span class="sxs-lookup"><span data-stu-id="d7280-179">notes</span></span>|<span data-ttu-id="d7280-180">String</span><span class="sxs-lookup"><span data-stu-id="d7280-180">String</span></span>|<span data-ttu-id="d7280-181">Заметки для приложения.</span><span class="sxs-lookup"><span data-stu-id="d7280-181">Notes for the app.</span></span> <span data-ttu-id="d7280-182">Наследуется от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d7280-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="d7280-183">publishingState</span></span>|[<span data-ttu-id="d7280-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d7280-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d7280-185">Состояние публикации для приложения.</span><span class="sxs-lookup"><span data-stu-id="d7280-185">The publishing state for the app.</span></span> <span data-ttu-id="d7280-186">Приложение невозможно назначить, если оно не опубликовано.</span><span class="sxs-lookup"><span data-stu-id="d7280-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d7280-187">Унаследованный от [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d7280-188">Возможные значения: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="d7280-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d7280-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d7280-189">committedContentVersion</span></span>|<span data-ttu-id="d7280-190">String</span><span class="sxs-lookup"><span data-stu-id="d7280-190">String</span></span>|<span data-ttu-id="d7280-191">Внутренняя версия подтвержденного содержимого.</span><span class="sxs-lookup"><span data-stu-id="d7280-191">The internal committed content version.</span></span> <span data-ttu-id="d7280-192">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d7280-193">fileName</span><span class="sxs-lookup"><span data-stu-id="d7280-193">fileName</span></span>|<span data-ttu-id="d7280-194">String</span><span class="sxs-lookup"><span data-stu-id="d7280-194">String</span></span>|<span data-ttu-id="d7280-195">Имя основного файла бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="d7280-195">The name of the main Lob application file.</span></span> <span data-ttu-id="d7280-196">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d7280-197">size</span><span class="sxs-lookup"><span data-stu-id="d7280-197">size</span></span>|<span data-ttu-id="d7280-198">Int64</span><span class="sxs-lookup"><span data-stu-id="d7280-198">Int64</span></span>|<span data-ttu-id="d7280-199">Общий размер, включая все отправленные файлы.</span><span class="sxs-lookup"><span data-stu-id="d7280-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="d7280-200">Наследуется от [mobileLobApp](../resources/intune-apps-mobilelobapp.md).</span><span class="sxs-lookup"><span data-stu-id="d7280-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d7280-201">commandLine</span><span class="sxs-lookup"><span data-stu-id="d7280-201">commandLine</span></span>|<span data-ttu-id="d7280-202">String</span><span class="sxs-lookup"><span data-stu-id="d7280-202">String</span></span>|<span data-ttu-id="d7280-203">Командная строка.</span><span class="sxs-lookup"><span data-stu-id="d7280-203">The command line.</span></span>|
|<span data-ttu-id="d7280-204">productCode</span><span class="sxs-lookup"><span data-stu-id="d7280-204">productCode</span></span>|<span data-ttu-id="d7280-205">String</span><span class="sxs-lookup"><span data-stu-id="d7280-205">String</span></span>|<span data-ttu-id="d7280-206">Код продукта.</span><span class="sxs-lookup"><span data-stu-id="d7280-206">The product code.</span></span>|
|<span data-ttu-id="d7280-207">productVersion</span><span class="sxs-lookup"><span data-stu-id="d7280-207">productVersion</span></span>|<span data-ttu-id="d7280-208">String</span><span class="sxs-lookup"><span data-stu-id="d7280-208">String</span></span>|<span data-ttu-id="d7280-209">Версия бизнес-приложения, к которому применяется MSI Windows Mobile.</span><span class="sxs-lookup"><span data-stu-id="d7280-209">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d7280-210">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="d7280-210">ignoreVersionDetection</span></span>|<span data-ttu-id="d7280-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7280-211">Boolean</span></span>|<span data-ttu-id="d7280-212">Логическое значение, позволяющее разрешить или запретить поиск установленного приложения по его версии.</span><span class="sxs-lookup"><span data-stu-id="d7280-212">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="d7280-213">Задайте значение true для бизнес-приложений MSI для Windows Mobile с функцией самостоятельного обновления.</span><span class="sxs-lookup"><span data-stu-id="d7280-213">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|



## <a name="response"></a><span data-ttu-id="d7280-214">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7280-214">Response</span></span>
<span data-ttu-id="d7280-215">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и обновленный объект [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d7280-215">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7280-216">Пример</span><span class="sxs-lookup"><span data-stu-id="d7280-216">Example</span></span>

### <a name="request"></a><span data-ttu-id="d7280-217">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7280-217">Request</span></span>
<span data-ttu-id="d7280-218">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7280-218">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```

### <a name="response"></a><span data-ttu-id="d7280-219">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7280-219">Response</span></span>
<span data-ttu-id="d7280-p119">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d7280-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1027

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true
}
```




