# <a name="windows10networkproxyserver-resource-type"></a>Тип ресурса windows10NetworkProxyServer

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Политика прокси-сервера сети.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|address|String|Адрес прокси-сервера. Укажите адрес в формате <server>\[":"<port>\]|
|exceptions|Коллекция String|Адреса, которые не должны использовать прокси-сервер. Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.|
|useForLocalAddresses|Boolean|Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```








