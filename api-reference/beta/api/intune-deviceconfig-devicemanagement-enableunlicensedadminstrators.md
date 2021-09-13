---
title: enableUnlicensedAdminstrators action
description: После включения пользователям, назначенным администраторами с помощью членов назначения ролей, больше не потребуется назначенная лицензия Intune. Для каждой группы безопасности AAD в назначении ролей может быть ограничено 350 нелицензионных прямых членов, но при необходимости для поддержки более 350 нелицензионных администраторов можно назначить несколько групп безопасности AAD. Лицензированные администраторы будут продолжать функционировать как есть в том, что транзитные членства применяются и не подлежат ограничению в 350 членов.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b62a4316f1faf04812571fdffed94d6b14ca12f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061172"
---
# <a name="enableunlicensedadminstrators-action"></a>enableUnlicensedAdminstrators action

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

После включения пользователям, назначенным администраторами с помощью членов назначения ролей, больше не потребуется назначенная лицензия Intune. Для каждой группы безопасности AAD в назначении ролей может быть ограничено 350 нелицензионных прямых членов, но при необходимости для поддержки более 350 нелицензионных администраторов можно назначить несколько групп безопасности AAD. Лицензированные администраторы будут продолжать функционировать как есть в том, что транзитные членства применяются и не подлежат ограничению в 350 членов.

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementServiceConfig.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableUnlicensedAdminstrators
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableUnlicensedAdminstrators
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 204 No Content
```



