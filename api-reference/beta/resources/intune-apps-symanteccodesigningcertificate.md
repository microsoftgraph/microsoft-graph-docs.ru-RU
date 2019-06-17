---
title: Тип ресурса symantecCodeSigningCertificate
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eb2df97c125827b54936ec5890923c799592ae61
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993314"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>Тип ресурса symantecCodeSigningCertificate

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md);|Чтение свойств и связей объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .|
|[Обновление symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md);|Обновление свойств объекта [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|содержимое|Binary|Сертификат подписи кода Windows Symantec в формате необработанных данных.|
|status|[Цертификатестатус](../resources/intune-apps-certificatestatus.md)|Состояние сертификата подготовлено или не подготовлено. Возможные значения: `notProvisioned`, `provisioned`.|
|password|Строка|Пароль, необходимый для PFX-файла.|
|subjectName|String|Имя субъекта для сертификата.|
|subject|String|Значение субъекта для сертификата.|
|Иссуернаме|String|Имя поставщика сертификата.|
|имени|String|Значение издателя для сертификата.|
|expirationDateTime|DateTimeOffset|Дата окончания срока действия сертификата.|
|Уплоаддатетиме|DateTimeOffset|Тип сертификата сопроектировании в качестве сертификата Symantec.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```





